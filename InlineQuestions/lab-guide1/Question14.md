## Metadata
Question Type : Single Choice

## Question
14. A junior admin asks "Can I rely on a vSphere snapshot as a long-term backup of a VM?" What is the correct answer?

## Options
Option 1: Yes — snapshots store a full copy of the VM and are safe to keep indefinitely
Option 2: No — snapshots store only changed blocks (delta) relative to the base disk; long-lived snapshots cause performance degradation, datastore space exhaustion, and increased risk during consolidation
Option 3: Yes, but only on NFS datastores
Option 4: Snapshots are functionally identical to backups taken by Veeam or Avamar

## Answers
Option 2 : 1

## Correct Answer Feedback
Correct. Snapshots are point-in-time delta files (sesparse on VMFS-6, redo logs on NFS). They depend on the base disk and grow as the VM writes. VMware best practice: keep snapshots no longer than 24-72 hours and never as primary backup.

## Incorrect Answer Feedback
Snapshots are not full copies and they do not survive deletion of the base VMDK. Datastore type does not change this. A real backup product creates an independent, restorable copy outside the production datastore.

## Tags
VMware
Snapshots
Backup
Foundational

## Number of Retries
0
