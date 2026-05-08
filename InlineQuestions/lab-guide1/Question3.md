## Metadata
Question Type : Multiple Choice

## Question
3. Which TWO of the following accurately describe ESXi 7.x architecture? (Select two)

## Options
Option 1: ESXi runs on a Linux kernel
Option 2: VMkernel is the proprietary VMware microkernel that schedules CPU, memory, and I/O for virtual machines
Option 3: Each running VM has its own user-world process called vmx that interfaces with VMkernel for hardware access
Option 4: Storage I/O from a guest OS bypasses VMkernel and goes directly to the HBA driver
Option 5: ESXi requires a separate service console partition that runs Red Hat Enterprise Linux

## Answers
Option 2 : 1
Option 3 : 1

## Correct Answer Feedback
Correct. VMkernel is VMware's purpose-built microkernel (Option 2) and each VM runs as a vmx user-world process that mediates hardware via VMkernel (Option 3).

## Incorrect Answer Feedback
ESXi does not run on Linux (Option 1 is wrong). All guest I/O traverses VMkernel (Option 4 is wrong). The Service Console was removed in ESXi 4.0+ — only the bare-metal hypervisor remains (Option 5 is wrong).

## Tags
VMware
vSphere
Architecture
Practitioner

## Number of Retries
0
