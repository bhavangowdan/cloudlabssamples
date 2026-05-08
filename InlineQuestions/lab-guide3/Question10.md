## Metadata
Question Type : Single Choice

## Question
10. What is a Solaris 11 non-kernel zone (brand: solaris)?

## Options
Option 1: A standalone Solaris install on a separate physical server
Option 2: An OS-level container that shares the global zone's kernel but has its own filesystem, process namespace, network identity, and configuration
Option 3: An LDOM
Option 4: A Branded zone for Linux compatibility

## Answers
Option 2 : 1

## Correct Answer Feedback
Correct. A Solaris non-kernel zone (default brand "solaris") is a kernel-shared OS-level partition. Many zones can run on one global zone. Branded zones (e.g., solaris10, lx) provide alternative environments.

## Incorrect Answer Feedback
A zone is virtualized, not on separate hardware (Option 1). LDOMs are hardware partitions (Option 3). lx-branded zones provide Linux compat (Option 4 is a different brand).

## Tags
Solaris
Zones
Foundational

## Number of Retries
0
