## Metadata
Question Type : Single Choice

## Question
12. Which utility on zLinux writes the boot record (kernel + initramfs + parmfile) to a DASD or FCP boot device, analogous to grub-install on x86?

## Options
Option 1: zipl
Option 2: grub2-mkconfig
Option 3: lilo
Option 4: bootctl

## Answers
Option 1 : 1

## Correct Answer Feedback
Correct. zipl ("z Initial Program Loader") is the s390x bootloader installer. After every kernel update on RHEL/SLES on Z you must explicitly run zipl — unlike x86, this is NOT automatic.

## Incorrect Answer Feedback
grub2-mkconfig and bootctl are x86 / UEFI tools. lilo is an obsolete x86 bootloader.

## Tags
zLinux
IPL
zipl
Foundational

## Number of Retries
0
