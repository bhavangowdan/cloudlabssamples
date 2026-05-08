## Metadata
Question Type : Single Choice

## Question
9. Which storage type on IBM Z uses fixed-block addressing similar to SCSI LUNs and is accessed via Fibre Channel Protocol?

## Options
Option 1: ECKD DASD
Option 2: FCP / SCSI-attached storage
Option 3: HiperSockets
Option 4: NSS (Named Saved Segment)

## Answers
Option 2 : 1

## Correct Answer Feedback
Correct. FCP attaches SCSI LUNs over Fibre Channel as fixed-block devices. zLinux multipath is provided by device-mapper-multipath stacked on /dev/sd* devices.

## Incorrect Answer Feedback
ECKD is variable-length count-key-data, the classical mainframe disk format. HiperSockets is in-memory networking. NSS is a memory-resident saved segment in z/VM, not storage.

## Tags
zLinux
Storage
FCP
Practitioner

## Number of Retries
0
