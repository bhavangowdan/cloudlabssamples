## Metadata
Question Type : Single Choice

## Question
20. Which is the recommended volume / filesystem stack for new Solaris 11 deployments?

## Options
Option 1: SVM (Solaris Volume Manager) for volumes + UFS for filesystems
Option 2: ZFS (combined volume management + filesystem with COW, snapshots, checksums)
Option 3: VxVM + VxFS only
Option 4: SVM + ZFS hybrid

## Answers
Option 2 : 1

## Correct Answer Feedback
Correct. ZFS is the default and recommended stack on Solaris 11. SVM/UFS remains supported for legacy compatibility but is not the choice for greenfield work.

## Incorrect Answer Feedback
SVM/UFS is legacy. VxVM/VxFS is third-party (Veritas). The hybrid is unnecessary because ZFS does both layers.

## Tags
Solaris
ZFS
SVM
Foundational

## Number of Retries
0
