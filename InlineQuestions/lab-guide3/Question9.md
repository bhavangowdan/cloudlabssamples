## Metadata
Question Type : Single Choice

## Question
9. When ZFS deduplication is enabled on a dataset under heavy write load, which is the PRIMARY performance constraint?

## Options
Option 1: Network bandwidth
Option 2: DDT (Deduplication Table) memory footprint and ARC pressure
Option 3: Compression CPU overhead
Option 4: ARC eviction policy

## Answers
Option 2 : 1

## Correct Answer Feedback
Correct. ZFS dedup requires the DDT to be resident in ARC (or hit L2ARC) for every write — roughly 320 bytes per unique block. On a multi-TB pool with small block sizes the DDT can be many GB. If it spills out of ARC, every write triggers a DDT lookup from disk, collapsing performance.

## Incorrect Answer Feedback
Compression is cheap (LZ4) and not the bottleneck. ARC eviction is downstream of the memory pressure dedup itself creates. Network is unrelated for local writes.

## Tags
Solaris
ZFS
Deduplication
Expert

## Number of Retries
0
