## Metadata
Question Type : Single Choice

## Question
3. A McKinsey client running RHEL on IBM Z notices that the s390x kernel includes drivers and device support that are absent on x86 RHEL. Which of the following s390x-specific features is correctly described?

## Options
Option 1: A kernel module to manage CCW (Channel Command Word) devices via the dasd_eckd_mod / zfcp drivers
Option 2: A built-in TPM 2.0 emulation layer that replaces s390 Crypto Express
Option 3: A native USB controller that exposes mainframe DASD as USB block devices
Option 4: A grub bootloader fork that writes boot records to DASD volumes

## Answers
Option 1 : 1

## Correct Answer Feedback
Correct. The s390x kernel ships dasd_eckd_mod (for ECKD DASD), zfcp (for FCP-attached SCSI LUNs), qeth (network), and other CCW-aware drivers — these are unique to the IBM Z platform and not present on x86 kernels.

## Incorrect Answer Feedback
TPM 2.0 emulation does not replace Crypto Express. There is no USB-DASD bridge. The Z-specific bootloader is zipl (not a grub fork) and writes to DASD via dedicated tooling.

## Tags
zLinux
KernelDrivers
Practitioner

## Number of Retries
0
