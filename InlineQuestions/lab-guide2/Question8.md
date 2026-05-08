## Metadata
Question Type : Single Choice

## Question
8. A McKinsey client wants the highest-performance configuration for a single-tenant high-throughput database workload on zLinux. Which deployment model gives the LOWEST hypervisor overhead?

## Options
Option 1: zLinux as a z/VM guest
Option 2: zLinux running natively in an LPAR (no z/VM)
Option 3: zLinux inside a Docker container on top of z/VM
Option 4: zLinux as a KVM-on-Z guest

## Answers
Option 2 : 1

## Correct Answer Feedback
Correct. Running Linux directly in an LPAR avoids the z/VM CP layer. PR/SM is firmware-level and very lightweight, so this is the closest-to-bare-metal option on Z. Trade-off: no fast cloning / no LGR.

## Incorrect Answer Feedback
z/VM and KVM-on-Z add a software hypervisor layer. Docker is a userland abstraction and does not bypass any hypervisor.

## Tags
zLinux
LPAR
Performance
Practitioner

## Number of Retries
0
