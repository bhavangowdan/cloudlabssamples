## Metadata
Question Type : Single Choice

## Question
23. A McKinsey client needs to migrate ~50 physical Windows Server 2019 hosts into a vSphere 7.x environment. VMware Converter Standalone has been deprecated. Which migration approach is currently supported and recommended for P2V at this scale?

## Options
Option 1: VMware vCenter Converter (still bundled with vSphere 7)
Option 2: A modern third-party tool (e.g., Veeam VM Conversion, Carbonite Migrate, Zerto) or in-place P2V via image-based backup-and-restore to a target VMDK
Option 3: Manual reinstall of the OS in a new VM and rsync of data
Option 4: Use Storage vMotion across the physical-to-virtual boundary

## Answers
Option 2 : 1

## Correct Answer Feedback
Correct. VMware Converter Standalone has been retired (last supported version 6.x). Modern P2V at scale uses third-party tools or backup-image rehydration into VMDKs. Architecture: snapshot physical -> ship to vSphere -> mount as VM.

## Incorrect Answer Feedback
Converter is no longer supported on current vSphere. Manual rebuild loses installed-app state. Storage vMotion only works between vSphere datastores — not across the physical/virtual boundary.

## Tags
VMware
Migration
P2V
Practitioner

## Number of Retries
0
