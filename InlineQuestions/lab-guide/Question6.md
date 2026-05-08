## Metadata
Question Type : Single Choice

## Question
6. What is the purpose of an AIX Virtual I/O Server (VIOS) in a PowerVM environment?

## Options
Option 1: To provide a graphical management console for AIX
Option 2: To own physical I/O adapters (FC HBAs, Ethernet NICs) and present virtualized I/O (vSCSI / NPIV / SEA) to client LPARs
Option 3: To run customer workloads at higher performance than regular LPARs
Option 4: To replace the HMC

## Answers
Option 2 : 1

## Correct Answer Feedback
Correct. The VIOS is a special-purpose AIX-based partition that owns the physical adapters and shares them with client LPARs as virtual SCSI, virtual Fibre Channel (NPIV), and Shared Ethernet Adapter (SEA).

## Incorrect Answer Feedback
The HMC provides management. VIOS itself does not run customer apps. VIOS does not replace the HMC — both coexist.

## Tags
AIX
VIOS
Practitioner

## Number of Retries
0
