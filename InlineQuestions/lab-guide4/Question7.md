## Metadata
Question Type : Single Choice

## Question
7. In JCL, what does DISP=(NEW,CATLG,DELETE) mean?

## Options
Option 1: Open existing dataset; catalog at end-of-step; delete on abnormal termination
Option 2: Allocate a new dataset; catalog it on normal step termination; delete it on abnormal step termination
Option 3: Allocate a new dataset; delete on normal end; catalog on abend
Option 4: Reuse an existing dataset; never catalog

## Answers
Option 2 : 1

## Correct Answer Feedback
Correct. DISP has three positional values: status (NEW/OLD/SHR/MOD), normal-end disposition (KEEP/CATLG/DELETE/PASS/UNCATLG), abnormal-end disposition (KEEP/CATLG/DELETE/UNCATLG). NEW=allocate, CATLG=keep+catalog on normal end, DELETE on abend.

## Incorrect Answer Feedback
The other interpretations swap status / normal / abnormal positions.

## Tags
zOS
JCL
DISP
Foundational

## Number of Retries
0
