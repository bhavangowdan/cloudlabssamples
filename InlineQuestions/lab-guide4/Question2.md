## Metadata
Question Type : Single Choice

## Question
2. On z/OS, what is the difference between virtual storage above the line and above the bar?

## Options
Option 1: Above the line is below 16 MB; above the bar is below 2 GB
Option 2: Above the line is between 16 MB and 2 GB (31-bit addressing); above the bar is above 2 GB (64-bit addressing)
Option 3: Above the line is for batch only; above the bar is for online only
Option 4: Both are obsolete with z/OS 2.5

## Answers
Option 2 : 1

## Correct Answer Feedback
Correct. The "line" is the 16 MB boundary (24-bit -> 31-bit addressing transition). The "bar" is the 2 GB boundary (31-bit -> 64-bit addressing). Programs and data classified as above-the-line / above-the-bar require the appropriate AMODE / RMODE settings.

## Incorrect Answer Feedback
Above the line is NOT below 16 MB (Option 1 confuses both). Workload type does not determine boundary placement (Option 3). Both concepts are still active in z/OS 2.5 (Option 4).

## Tags
zOS
Storage
AMODE
Foundational

## Number of Retries
0
