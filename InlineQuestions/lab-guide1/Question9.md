## Metadata
Question Type : Single Choice

## Question
9. You need a vSphere HA cluster to tolerate the simultaneous failure of an entire rack containing 3 of its 9 ESXi hosts. Which HA capability addresses this directly?

## Options
Option 1: Increase HA Restart Priority for production VMs
Option 2: Enable Proactive HA
Option 3: Use HA "Failures and responses" with Host Isolation Response set to Power Off
Option 4: Configure HA Admission Control with "Failures cluster tolerates" set appropriately and enable Fault Domains so the cluster understands the rack topology

## Answers
Option 4 : 1

## Correct Answer Feedback
Correct. HA Fault Domains (introduced as part of vSAN Stretched/Fault Domain awareness, also leveraged by HA topology) lets HA distribute restart capacity such that rack failure does not exhaust failover headroom. Combined with the right "Failures cluster tolerates" value, HA can place restart capacity outside the failed fault domain.

## Incorrect Answer Feedback
Restart priority only orders recovery of VMs, not capacity. Proactive HA acts on hardware degradation signals (e.g., Dell OMSA), not rack failure. Host isolation response handles network partitions, not rack failure.

## Tags
VMware
HA
FaultDomains
Expert

## Number of Retries
0
