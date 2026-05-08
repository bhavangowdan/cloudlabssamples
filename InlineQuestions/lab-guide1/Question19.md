## Metadata
Question Type : Single Choice

## Question
19. A 3-node vSAN cluster is reporting "reduced redundancy" on 40% of VM objects. The vSAN health check shows one capacity disk on host esx-02 has elevated latency (>50ms) and read errors. What is the SAFEST first step?

## Options
Option 1: Pull the disk physically and replace it immediately
Option 2: Place the disk in maintenance mode with "Full data migration" so vSAN evacuates components, then replace
Option 3: Disable vSAN cluster maintenance mode and reboot esx-02
Option 4: Reduce the storage policy FTT to 0 to clear the alert

## Answers
Option 2 : 1

## Correct Answer Feedback
Correct. Maintenance Mode with Full Data Migration triggers an orderly evacuation of components from the failing disk to other healthy disks/hosts. Pulling the disk hot would cause vSAN to rebuild from the surviving copy under emergency conditions.

## Incorrect Answer Feedback
Hot-pulling the disk causes immediate degraded state across affected objects. Rebooting the host does not address the failing disk. Reducing FTT to 0 destroys redundancy and is never the answer to a hardware failure.

## Tags
VMware
vSAN
Maintenance
Practitioner

## Number of Retries
0
