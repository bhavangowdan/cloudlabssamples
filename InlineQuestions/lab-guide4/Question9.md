## Metadata
Question Type : Multiple Choice

## Question
9. Which TWO of the following are valid uses of cataloged procedures (PROCs) in JCL? (Select two)

## Options
Option 1: Define a reusable set of EXEC + DD steps that callers invoke with parameter overrides
Option 2: Replace JCL entirely with shell scripts
Option 3: Allow operator-only commands to bypass RACF
Option 4: Standardize batch DD allocations and program invocations across many jobs
Option 5: Disable spool processing for all jobs in the system

## Answers
Option 1 : 1
Option 4 : 1

## Correct Answer Feedback
Correct. PROCs encapsulate reusable JCL (Option 1) and standardize DD/EXEC patterns across many jobs (Option 4). PROCs live in JCL libraries (PROCLIB) and are invoked by EXEC PROC=name.

## Incorrect Answer Feedback
PROCs do not replace JCL — they ARE JCL. They do not bypass security. They do not affect spool.

## Tags
zOS
JCL
PROC
Practitioner

## Number of Retries
0
