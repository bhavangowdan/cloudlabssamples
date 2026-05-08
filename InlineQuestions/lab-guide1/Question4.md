## Metadata
Question Type : Single Choice

## Question
4. You need to evacuate every running VM from an ESXi host before applying firmware updates, with zero downtime to applications. Which feature is designed for this?

## Options
Option 1: Storage vMotion
Option 2: vMotion (host) with Maintenance Mode
Option 3: VMware Fault Tolerance
Option 4: Cold migration

## Answers
Option 2 : 1

## Correct Answer Feedback
Correct. Placing the host into Maintenance Mode triggers DRS (or admin-driven) vMotions to evacuate all powered-on VMs to other hosts in the cluster with no guest downtime.

## Incorrect Answer Feedback
Storage vMotion moves VM disk files between datastores (not hosts). Fault Tolerance keeps a synchronized secondary VM but is not the evacuation mechanism. Cold migration requires the VM to be powered off.

## Tags
VMware
vMotion
Foundational

## Number of Retries
0
