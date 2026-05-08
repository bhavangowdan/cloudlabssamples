## Metadata
Question Type : Text Input

## Question
21. Briefly explain the difference between deploying a Linux workload directly in an LPAR vs. as a z/VM guest. Give one workload type that is a better fit for each.

## Options
N/A

## Answers
^(?i)(lpar|pr/sm|z/vm|zvm|guest|hypervisor|vm|virtual|workload)$

## Correct Answer Feedback
An LPAR is a hardware-level partition managed by PR/SM (firmware hypervisor) — it gets dedicated or shared physical CPU, memory, and I/O directly from the CPC. A z/VM guest is a virtual machine running under the z/VM hypervisor, which itself runs inside an LPAR. z/VM provides finer-grained resource sharing, overcommitment, fast provisioning, and live relocation across SSI members. Linux workloads are a better fit for an LPAR when maximum and predictable performance, low overhead, or dedicated hardware resources are required. z/VM guests are better suited for environments that need to run many Linux instances efficiently with flexible resource sharing and rapid lifecycle management.

## Incorrect Answer Feedback
A common misunderstanding is treating LPARs and z/VM guests as the same type of virtualization. LPARs are hardware-based partitions managed by firmware (PR/SM), while z/VM is a software hypervisor that runs within an LPAR to host multiple virtual machines.

## Tags
zLinux
LPAR
zVM
Practitioner

## Number of Retries
0
