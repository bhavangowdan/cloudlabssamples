## Metadata
Question Type : Single Choice

## Question
16. What is USS (UNIX System Services) on z/OS?

## Options
Option 1: A separate Linux LPAR
Option 2: A POSIX-compliant UNIX environment hosted INSIDE the z/OS kernel, with a hierarchical filesystem (zFS / HFS), shell (e.g., /bin/sh), and full UNIX system calls — accessible via OMVS / ish from TSO or directly via SSH
Option 3: A z/VM guest running Linux
Option 4: An emulator that runs UNIX binaries unchanged

## Answers
Option 2 : 1

## Correct Answer Feedback
Correct. USS is a fully integrated UNIX subsystem in z/OS — it shares the same SAF security, the same address-space dispatch, but exposes a POSIX kernel API and a hierarchical filesystem. Java and many open-source ports on z/OS run on USS.

## Incorrect Answer Feedback
USS is part of z/OS, not a separate OS or LPAR. It is not an emulator.

## Tags
zOS
USS
Foundational

## Number of Retries
0
