## Metadata
Question Type : Multiple Choice

## Question
19. Which of the following are valid uses of the AIX errpt command? (Select all that apply)

## Options
Option 1: View hardware error log entries (e.g., disk read failures, memory errors)
Option 2: View software error log entries from the kernel and subsystems
Option 3: Generate a detailed report with errpt -a for a specific identifier
Option 4: Configure error notification methods
Option 5: Edit the contents of /var/adm/ras/errlog directly

## Answers
Option 1 : 1
Option 2 : 1
Option 3 : 1

## Correct Answer Feedback
Correct. errpt reads /var/adm/ras/errlog (binary) and displays HW + SW errors (Options 1, 2). errpt -a shows full detail (Option 3).

## Incorrect Answer Feedback
Notification is configured via the errnotify ODM class (using odmadd), not errpt itself (Option 4 wrong). The errlog is binary and must be cleared with errclear, not edited (Option 5 wrong).

## Tags
AIX
errpt
Practitioner

## Number of Retries
0
