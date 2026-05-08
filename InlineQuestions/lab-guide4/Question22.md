## Metadata
Question Type : Single Choice

## Question
22. Which RACF profile would you check to determine whether userid TMHASSEM has UPDATE access to dataset PROD.PAYROLL.MASTER?

## Options
Option 1: The RACF user profile for TMHASSEM
Option 2: The most-specific dataset profile that matches PROD.PAYROLL.MASTER (could be a discrete profile, or a generic like PROD.PAYROLL.* or PROD.**)
Option 3: The RACF group profile for the user's default group
Option 4: The PROD resource class profile

## Answers
Option 2 : 1

## Correct Answer Feedback
Correct. RACF dataset access is governed by the most-specific matching profile in the DATASET class — discrete profile if it exists, else best generic match. Use LISTDSD 'PROD.PAYROLL.MASTER' to find it. The user profile holds attributes; group profile is checked indirectly via PERMITs on the dataset profile. PROD is not a class.

## Incorrect Answer Feedback
The user/group profiles do not directly hold dataset access. RACF resource classes are things like FACILITY, OPERCMDS — not "PROD".

## Tags
zOS
RACF
Practitioner

## Number of Retries
0
