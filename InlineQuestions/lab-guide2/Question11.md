## Metadata
Question Type : Single Choice

## Question
11. A Db2 LUW workload on RHEL 8 in an IBM Z LPAR is experiencing high I/O latency. iostat shows 95%+ utilization on ECKD DASD volumes, but CPU is only 40%. Which Z-specific feature should you evaluate to increase parallel I/O throughput PER DASD volume without adding new physical devices?

## Options
Option 1: HyperPAV (Hyper Parallel Access Volumes) - aliases UCBs to allow multiple concurrent I/Os to the same DASD
Option 2: Storage vMotion to a different datastore
Option 3: ZFS deduplication
Option 4: GFS2 clustered filesystem

## Answers
Option 1 : 1

## Correct Answer Feedback
Correct. HyperPAV uses dynamic UCB aliases so multiple I/Os can be in flight to the same DASD volume in parallel — a classic remedy for ECKD device-level serialization. It does not require new disks.

## Incorrect Answer Feedback
Storage vMotion is VMware. ZFS dedup is a Solaris/Linux feature unrelated to ECKD. GFS2 is a Linux clustered filesystem, not a Z parallelism mechanism.

## Tags
zLinux
Storage
HyperPAV
Expert

## Number of Retries
0
