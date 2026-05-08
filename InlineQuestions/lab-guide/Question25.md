## Metadata
Question Type : Single Choice

## Question
25. On AIX 7.x with Enhanced RBAC enabled, which command is used to assign a role to a user?

## Options
Option 1: chuser roles=<role> <username>
Option 2: chmod
Option 3: usermod -aG <role> <username>
Option 4: setrole <role> <username>

## Answers
Option 1 : 1

## Correct Answer Feedback
Correct. On AIX, role assignments are stored in the user attributes; chuser roles=<role> <username> assigns. Subsequent login picks up the role; swrole switches to it within a session.

## Incorrect Answer Feedback
chmod is for file permissions. usermod -aG is the Linux idiom for groups. setrole is the active-role switch in some POSIX systems but not the AIX assignment command.

## Tags
AIX
RBAC
Practitioner

## Number of Retries
0
