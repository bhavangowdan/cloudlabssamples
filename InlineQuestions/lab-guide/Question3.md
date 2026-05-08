## Metadata
Question Type : Single Choice

## Question
3. Which AIX construct is a software partition INSIDE a single AIX instance, sharing the global kernel but with its own filesystem namespace and process tree?

## Options
Option 1: WPAR (Workload Partition)
Option 2: LPAR (Logical Partition)
Option 3: Solaris Zone
Option 4: VIO Server

## Answers
Option 1 : 1

## Correct Answer Feedback
Correct. WPAR (Workload Partition) is a software-level partitioning mechanism within one AIX instance — analogous to a Solaris non-kernel zone or a Linux container. It shares the AIX kernel but isolates filesystem, process namespace, and network identity.

## Incorrect Answer Feedback
LPAR is a hardware partition created by PHYP. Solaris Zones is the Solaris equivalent (different OS). VIO Server is a special LPAR type that virtualizes I/O.

## Tags
AIX
WPAR
LPAR
Foundational

## Number of Retries
0
