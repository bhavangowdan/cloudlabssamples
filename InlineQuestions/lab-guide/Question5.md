## Metadata
Question Type : Multiple Choice

## Question
5. Which TWO of the following statements about WPARs are correct? (Select two)

## Options
Option 1: A WPAR shares the AIX kernel of its hosting global LPAR
Option 2: Each WPAR can run a different AIX TL/SP than its host
Option 3: A WPAR has its own filesystem, process namespace, and (optionally) IP stack
Option 4: WPARs require dedicated POWER hardware
Option 5: WPARs cannot be moved between hosts

## Answers
Option 1 : 1
Option 3 : 1

## Correct Answer Feedback
Correct. WPARs share the kernel (Option 1) and have their own filesystem/process/network namespace (Option 3). They are software partitions inside one AIX kernel.

## Incorrect Answer Feedback
WPARs run the same kernel/TL/SP as their host (Option 2 wrong). They run inside a regular LPAR, no special hardware (Option 4 wrong). Live Application Mobility (LAM) historically supported moving WPARs (Option 5 wrong).

## Tags
AIX
WPAR
Practitioner

## Number of Retries
0
