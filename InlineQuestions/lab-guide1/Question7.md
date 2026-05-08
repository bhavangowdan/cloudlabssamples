## Metadata
Question Type : Single Choice

## Question
7. A 6-node ESXi cluster has vSphere HA enabled. One ESXi host fails (PSOD). What does HA do?

## Options
Option 1: Live-migrates the VMs from the failed host to surviving hosts using vMotion
Option 2: Restarts the failed host's VMs on surviving hosts according to restart priority
Option 3: Powers down the failed host's VMs and waits for an admin to recover them
Option 4: Triggers a Site Recovery Manager failover to the DR site

## Answers
Option 2 : 1

## Correct Answer Feedback
Correct. vSphere HA detects host failure via the master/slave heartbeat protocol and restarts (cold-boots) the affected VMs on remaining hosts. vMotion cannot be used because the source host is dead.

## Incorrect Answer Feedback
vMotion requires a live source host (Option 1 wrong). HA restarts VMs automatically; no admin intervention is required by default (Option 3 wrong). SRM is a separate product for cross-site DR (Option 4 wrong).

## Tags
VMware
HA
Foundational

## Number of Retries
0
