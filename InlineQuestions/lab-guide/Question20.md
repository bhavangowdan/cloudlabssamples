## Metadata
Question Type : Single Choice

## Question
20. An AIX admin runs `errpt | head` and sees an entry with class=H, type=PERM, resource=hdisk3, description="DISK OPERATION ERROR". Which is the MOST LIKELY interpretation?

## Options
Option 1: An informational message — no action needed
Option 2: A permanent hardware error on hdisk3 (PERM type means the error has not been recovered transparently); investigate the SAN path / physical disk and check MPIO state
Option 3: A temporary error that auto-cleared
Option 4: A user permission error

## Answers
Option 2 : 1

## Correct Answer Feedback
Correct. PERM (permanent) errors did not transparently recover and require investigation. class=H = hardware. The likely cause: failed SAN path, bad cable, or failing physical disk. Check lspath / lsmpio and mpio status, then escalate to storage team.

## Incorrect Answer Feedback
Informational entries are TYPE=INFO. PERM is NOT temporary. errpt is a hardware/software error log, not a user permission log.

## Tags
AIX
errpt
Hardware
Practitioner

## Number of Retries
0
