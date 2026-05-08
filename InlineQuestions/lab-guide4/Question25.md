## Metadata
Question Type : Single Choice

## Question
25. What is the relationship between SMF and RMF on z/OS?

## Options
Option 1: SMF (System Management Facilities) records system events / metrics into log datasets (SMF type 30 = job/step, 70-78 = RMF, 110 = CICS, 100-102 = DB2, etc.); RMF (Resource Measurement Facility) is the IBM performance reporter that uses SMF type 70-78 (and gathers its own data) to produce performance and capacity reports
Option 2: SMF is the same as RMF
Option 3: RMF is for security; SMF is for performance
Option 4: SMF is z/OS 2.5 only; RMF is older

## Answers
Option 1 : 1

## Correct Answer Feedback
Correct. SMF is the system-wide event recorder — virtually every subsystem writes SMF records. RMF gathers performance data (CPU, I/O, paging, sysplex) and writes SMF type 70-78. Reports are produced by RMF Postprocessor or the Monitor III online viewer.

## Incorrect Answer Feedback
Security audit goes to SMF (type 80 for RACF), but RMF is performance-focused. Both have been around for decades.

## Tags
zOS
SMF
RMF
Practitioner

## Number of Retries
0
