## Metadata
Question Type : Single Choice

## Question
6. Which statement about a ZFS snapshot is correct?

## Options
Option 1: A snapshot is a writable copy of a dataset
Option 2: A snapshot is a read-only, near-instantaneous, copy-on-write point-in-time view of a dataset that consumes only changed blocks
Option 3: A snapshot is a full block-level copy that doubles space usage
Option 4: A snapshot can only be created when the dataset is unmounted

## Answers
Option 2 : 1

## Correct Answer Feedback
Correct. ZFS snapshots are read-only, instant, and copy-on-write. They share blocks with the live dataset and consume only blocks that diverge after the snapshot is taken.

## Incorrect Answer Feedback
Writable copies are clones (created from snapshots). Snapshots do not double space. They can be taken on mounted, active datasets.

## Tags
Solaris
ZFS
Snapshots
Foundational

## Number of Retries
0
