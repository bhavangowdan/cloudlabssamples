## Metadata
Question Type : Single Choice

## Question
5. A vMotion operation between two ESXi hosts in the same cluster fails with the error "The source detected that the destination failed to resume." Which is the MOST likely root cause to investigate first?

## Options
Option 1: The source host has insufficient memory headroom
Option 2: CPU feature mismatch between source and destination hosts (no EVC, or EVC baseline too high)
Option 3: The VM has a snapshot
Option 4: The destination host's vMotion VMkernel adapter has a different MTU

## Answers
Option 2 : 1

## Correct Answer Feedback
Correct. "Failed to resume on destination" classically points to CPU feature incompatibility — the running VM was using a CPU instruction not exposed on the target. Enable EVC at the lowest common baseline and retry.

## Incorrect Answer Feedback
Memory pressure causes a different error (insufficient resources). Snapshots do not block vMotion. MTU mismatch causes vMotion to stall during memory copy, not fail at resume.

## Tags
VMware
vMotion
EVC
Practitioner

## Number of Retries
0
