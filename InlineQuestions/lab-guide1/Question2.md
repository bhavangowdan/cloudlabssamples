## Metadata
Question Type : Single Choice

## Question
2. On an ESXi 7.x host, which kernel-level process is the primary management agent that vCenter Server communicates with to perform VM operations and configuration changes?

## Options
Option 1: vmkernel
Option 2: hostd
Option 3: vpxa
Option 4: vmx

## Answers
Option 3 : 1

## Correct Answer Feedback
Correct. vpxa is the vCenter agent on each ESXi host. It receives instructions from vCenter (vpxd) and forwards them to hostd, which performs the actual host operations.

## Incorrect Answer Feedback
vmkernel is the hypervisor itself, hostd is the local host daemon (used by direct host clients), and vmx is the per-VM process. vCenter speaks to ESXi via vpxa.

## Tags
VMware
vSphere
Architecture
Practitioner

## Number of Retries
0
