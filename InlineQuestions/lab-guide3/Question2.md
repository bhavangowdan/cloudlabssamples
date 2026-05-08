## Metadata
Question Type : Single Choice

## Question
2. Which Oracle Solaris feature provides hardware-assisted partitioning ON SPARC servers, allowing multiple Solaris instances on a single physical server with each having its own kernel?

## Options
Option 1: Solaris Zones
Option 2: LDOMs (Oracle VM Server for SPARC, also known as Logical Domains)
Option 3: SVM (Solaris Volume Manager)
Option 4: SMF (Service Management Facility)

## Answers
Option 2 : 1

## Correct Answer Feedback
Correct. LDOMs (Oracle VM Server for SPARC) is the hardware-assisted hypervisor on SPARC T-series and M-series. Each LDOM has its own Solaris kernel and resources are virtualized via the SPARC firmware hypervisor.

## Incorrect Answer Feedback
Zones share a kernel (different mechanism). SVM is for storage volumes. SMF is service management.

## Tags
Solaris
LDOM
Foundational

## Number of Retries
0
