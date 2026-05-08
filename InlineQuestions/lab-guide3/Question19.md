## Metadata
Question Type : Single Choice

## Question
19. A Solaris 11 application is intermittently slow. You suspect a specific kernel function is taking variable time. Which DTrace probe-pair lets you measure how long a kernel function takes per invocation?

## Options
Option 1: profile-100hz alone
Option 2: fbt:::entry / fbt:::return on the function name, computing timestamp delta in the action block
Option 3: syscall::open:entry only
Option 4: io::done

## Answers
Option 2 : 1

## Correct Answer Feedback
Correct. The fbt provider exposes entry and return probes for every kernel function. Capture timestamp on entry, compute delta on return: `fbt::funcname:entry { self->t = timestamp; } fbt::funcname:return /self->t/ { @ = quantize(timestamp - self->t); self->t = 0; }`.

## Incorrect Answer Feedback
profile is sampling, not paired entry/return. syscall::open:entry only fires on one specific syscall. io::done only fires for block I/O completions.

## Tags
Solaris
DTrace
fbt
Expert

## Number of Retries
0
