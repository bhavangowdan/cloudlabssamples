## Metadata
Question Type : Single Choice

## Question
13. In AIX LVM, what is the relationship between a Physical Partition (PP) and a Logical Partition (LP) in a mirrored Logical Volume with copy count = 2?

## Options
Option 1: 1 LP maps to 1 PP
Option 2: 1 LP maps to 2 PPs (one per mirror copy)
Option 3: 1 PP maps to multiple LPs
Option 4: LP and PP are unrelated abstractions

## Answers
Option 2 : 1

## Correct Answer Feedback
Correct. Mirroring at the LV level means each LP is backed by N PPs, where N = copy count. With copies=2, every LP has 2 PPs (ideally on different PVs / failure groups).

## Incorrect Answer Feedback
Without mirroring, LP:PP is 1:1 (Option 1 wrong for mirrored). Reverse direction is incorrect (Option 3). LP and PP are tightly related (Option 4 wrong).

## Tags
AIX
LVM
Foundational

## Number of Retries
0
