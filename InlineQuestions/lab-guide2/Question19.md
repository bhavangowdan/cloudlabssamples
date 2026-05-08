## Metadata
Question Type : Single Choice

## Question
19. A zLinux guest under z/VM panics intermittently. Which kernel parameter ensures kdump is invoked and a vmcore is captured for later analysis with the crash utility?

## Options
Option 1: panic=0
Option 2: crashkernel=auto (or a sized value such as crashkernel=256M-:256M) plus an active kdump.service
Option 3: kpti=on
Option 4: zswap.enabled=1

## Answers
Option 2 : 1

## Correct Answer Feedback
Correct. crashkernel= reserves memory for the kdump kernel that boots in place of the panicked one to capture the dump. kdump.service must be enabled and the dump target (FCP/DASD/NFS) configured.

## Incorrect Answer Feedback
panic=0 disables auto-reboot on panic but does not configure kdump. kpti and zswap are unrelated.

## Tags
zLinux
Dump
kdump
Expert

## Number of Retries
0
