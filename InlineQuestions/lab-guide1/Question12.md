## Metadata
Question Type : Single Choice

## Question
12. Which of the following is TRUE about a VMFS-6 datastore?

## Options
Option 1: It is a network file system mounted from a NAS over NFSv3
Option 2: It is a clustered block filesystem on a SCSI/FC/iSCSI LUN that supports concurrent access from multiple ESXi hosts
Option 3: It can only be mounted by one ESXi host at a time
Option 4: It does not support thin-provisioned VMDKs

## Answers
Option 2 : 1

## Correct Answer Feedback
Correct. VMFS is VMware's high-performance clustered filesystem layered on a block LUN. Multiple ESXi hosts can mount the same VMFS datastore simultaneously, with locking coordinated via SCSI-3 reservations or ATS (VAAI Atomic Test & Set).

## Incorrect Answer Feedback
NFS datastores are file-level (not VMFS). VMFS is explicitly designed for cluster-wide concurrent access. Thin-provisioned VMDKs are fully supported on VMFS.

## Tags
VMware
Storage
VMFS
Foundational

## Number of Retries
0
