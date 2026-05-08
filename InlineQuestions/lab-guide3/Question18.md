## Metadata
Question Type : Single Choice

## Question
18. Which DTrace provider would you use to trace every system call entry made by PID 1234 with its arguments?

## Options
Option 1: fbt (Function Boundary Tracing)
Option 2: syscall provider with /pid == 1234/ predicate
Option 3: profile provider at 100Hz
Option 4: io provider

## Answers
Option 2 : 1

## Correct Answer Feedback
Correct. The syscall provider has entry/return probes for every syscall. With predicate /pid == 1234/, it filters to that process. Example: dtrace -n 'syscall:::entry /pid == 1234/ { @[probefunc] = count(); }'.

## Incorrect Answer Feedback
fbt traces kernel function boundaries (lower-level than syscall). profile is sampling-based, not syscall-driven. io is for block I/O events.

## Tags
Solaris
DTrace
syscall
Practitioner

## Number of Retries
0
