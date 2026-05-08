## Metadata
Question Type : Single Choice

## Question
21. A McKinsey client running 200 VMs in an on-prem vSphere estate wants to lift-and-shift to Azure VMware Solution (AVS). Which of the following migration tools is MOST appropriate to migrate large numbers of VMs with minimal downtime?

## Options
Option 1: Azure Site Recovery (ASR)
Option 2: VMware HCX
Option 3: Robocopy / rsync inside each guest OS
Option 4: Cold export to OVF, upload to Azure Blob, re-import

## Answers
Option 2 : 1

## Correct Answer Feedback
Correct. VMware HCX is purpose-built for hybrid VMware migration. It supports bulk migration, live migration (vMotion-style), and cross-cloud migration (on-prem to AVS / VMC) with WAN optimization. AVS includes an HCX Advanced license.

## Incorrect Answer Feedback
ASR works for IaaS-to-Azure (Hyper-V/vSphere into Azure VMs), not VMware-on-Azure preserving VMware semantics. Guest-OS file copy is not VM migration. Cold OVF is technically possible but slow and incurs full downtime.

## Tags
VMware
AVS
HCX
Practitioner

## Number of Retries
0
