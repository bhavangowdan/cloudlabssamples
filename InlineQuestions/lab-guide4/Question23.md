## Metadata
Question Type : Single Choice

## Question
23. Which RACF command grants user TMHASSEM READ access to dataset profile PROD.PAYROLL.MASTER?

## Options
Option 1: PERMIT 'PROD.PAYROLL.MASTER' ID(TMHASSEM) ACCESS(READ)
Option 2: ALTUSER TMHASSEM READ('PROD.PAYROLL.MASTER')
Option 3: ADDSD 'PROD.PAYROLL.MASTER' READ(TMHASSEM)
Option 4: SETROPTS GENERIC(DATASET) ACCESS(READ)

## Answers
Option 1 : 1

## Correct Answer Feedback
Correct. PERMIT is the canonical RACF command to grant access. ID(user-or-group) ACCESS(READ/UPDATE/CONTROL/ALTER). The dataset profile must already exist (or be created with ADDSD).

## Incorrect Answer Feedback
ALTUSER modifies user attributes, not access. ADDSD adds dataset profiles but doesn't grant access. SETROPTS is system-wide options.

## Tags
zOS
RACF
PERMIT
Practitioner

## Number of Retries
0
