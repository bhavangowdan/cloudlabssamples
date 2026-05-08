## Metadata
Question Type : Single Choice

## Question
10. You manage a vSphere Distributed Switch (VDS) shared by 12 ESXi hosts. Which statement about VDS port group configuration is correct?

## Options
Option 1: Each host maintains its own copy of port group settings, and changes must be applied per-host
Option 2: Port group settings are configured centrally on vCenter and pushed to all member hosts; if vCenter is offline, hosts continue forwarding using last-known config
Option 3: VDS port groups can only be edited by directly SSHing into each ESXi host
Option 4: VDS port groups disappear if vCenter Server becomes unavailable

## Answers
Option 2 : 1

## Correct Answer Feedback
Correct. VDS configuration is stored centrally on vCenter and pushed to hosts. Hosts cache the configuration locally so that data-plane forwarding continues even when vCenter (the management plane) is unreachable.

## Incorrect Answer Feedback
Per-host configuration is the model for vSphere Standard Switch (VSS), not VDS. VDS is configured in vCenter only. The data plane survives vCenter outages.

## Tags
VMware
Networking
VDS
Practitioner

## Number of Retries
0
