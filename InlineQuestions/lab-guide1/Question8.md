## Metadata
Question Type : Single Choice

## Question
8. A vSphere HA cluster has Admission Control set to "Cluster resource percentage" reserving 25% CPU and 25% memory. The cluster has 4 hosts. A user attempts to power on a new VM with a 16 GB memory reservation, but the operation fails with "Insufficient resources to satisfy configured failover level for vSphere HA". Why?

## Options
Option 1: One of the hosts is in maintenance mode
Option 2: Powering on the VM would push committed reservations above the 75% threshold, leaving less than 25% headroom for the configured failover level
Option 3: DRS is set to manual and won't approve the placement
Option 4: The VM's CPU reservation conflicts with vMotion EVC

## Answers
Option 2 : 1

## Correct Answer Feedback
Correct. Cluster resource percentage admission control reserves the configured percentage as failover capacity. Power-on operations are denied if they would consume reservation capacity protected for failover, regardless of unreserved free RAM.

## Incorrect Answer Feedback
Maintenance mode would reduce available capacity but the error specifically references HA failover level. DRS automation level affects placement, not admission. EVC governs CPU compatibility for vMotion, not power-on.

## Tags
VMware
HA
AdmissionControl
Practitioner

## Number of Retries
0
