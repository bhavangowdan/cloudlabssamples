## Metadata
Question Type : Text Input

## Question
13. A zLinux guest under z/VM fails to IPL after a kernel update. The console shows the kernel loads but then halts before reaching the initramfs. Briefly describe the FIRST artifact you would inspect and why.

## Options
N/A

## Answers
^(?i)(parmfile|initramfs|zipl|kernel|cmdline|dasd|rootfs)$

## Correct Answer Feedback
nspect the parmfile (kernel parameters) referenced by the zipl boot loader configuration in /etc/zipl.conf. On IBM Z systems, zipl writes the kernel, initramfs, and parmfile to the boot device. If the kernel update modified or invalidated parmfile contents such as an incorrect root= UUID or missing rd.zfcp= or rd.dasd= parameters, the kernel cannot locate or mount the root filesystem and halts before reaching the initramfs stage. It is also important to verify that zipl was explicitly run after the kernel package installation, as this step is mandatory on RHEL and SLES for IBM Z.

## Incorrect Answer Feedback
A common incorrect assumption is that GRUB configuration applies on IBM Z. GRUB is not used on s390x systems. The supported and required boot loader is zipl, which must be manually executed after every kernel update to correctly write boot artifacts to the IPL device.

## Tags
zLinux
IPL
zipl
Expert

## Number of Retries
0
