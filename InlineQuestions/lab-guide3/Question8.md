## Metadata
Question Type : Single Choice

## Question
8. Which ZFS command set replicates a dataset (and its snapshots) from one host to another over SSH?

## Options
Option 1: zfs send <snapshot> | ssh user@target zfs receive <dataset>
Option 2: rsync -av /pool/dataset target:/pool/
Option 3: zpool replicate
Option 4: zfs mirror --to user@target

## Answers
Option 1 : 1

## Correct Answer Feedback
Correct. zfs send/receive is the canonical, block-aware replication mechanism. It transmits a stream of dataset changes (full or incremental between two snapshots) and is far more efficient than file-level rsync.

## Incorrect Answer Feedback
rsync works but is file-level (slower, no preservation of ZFS properties / snapshots). zpool replicate and zfs mirror are not commands.

## Tags
Solaris
ZFS
Replication
Practitioner

## Number of Retries
0
