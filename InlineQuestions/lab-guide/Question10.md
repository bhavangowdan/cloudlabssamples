## Metadata
Question Type : Multiple Choice

## Question
10. Which of the following are REQUIRED for a successful Live Partition Mobility (LPM) operation between two POWER frames? (Select all that apply)

## Options
Option 1: Source and target frames managed by the same HMC (or HMCs in a cooperative pair)
Option 2: Both frames at compatible POWER processor levels and firmware levels
Option 3: Source LPAR using only NPIV (no vSCSI) for storage
Option 4: Source LPAR storage accessible from both frames' VIOSes
Option 5: Source LPAR memory size smaller than target frame's free memory

## Answers
Option 1 : 1
Option 2 : 1
Option 4 : 1
Option 5 : 1

## Correct Answer Feedback
Correct. LPM requires HMC visibility (Option 1), processor/firmware compatibility (Option 2), shared storage access from both ends' VIOSes via NPIV or vSCSI (Option 4), and enough target memory (Option 5).

## Incorrect Answer Feedback
vSCSI is supported for LPM as long as backing devices are accessible from both VIOSes — NPIV is not strictly required (Option 3 wrong).

## Tags
AIX
LPM
Expert

## Number of Retries
0
