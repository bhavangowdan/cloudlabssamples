## Metadata
Question Type : Single Choice

## Question
20. In NSX-T, which component implements distributed firewalling at the vNIC level of each VM, evaluating policies in the hypervisor before traffic hits the wire?

## Options
Option 1: Edge Transport Node
Option 2: NSX Manager
Option 3: Distributed Firewall (DFW) running in the kernel of each ESXi transport node
Option 4: NSX Cloud Service Manager

## Answers
Option 3 : 1

## Correct Answer Feedback
Correct. NSX Distributed Firewall enforces stateful policy in the hypervisor kernel at the vNIC level — east-west traffic between VMs on the same host is filtered without leaving the host.

## Incorrect Answer Feedback
Edge Transport Nodes handle north-south and stateful services like NAT/VPN. NSX Manager is the management plane. CSM is for public-cloud NSX integration.

## Tags
VMware
NSX
DFW
Practitioner

## Number of Retries
0
