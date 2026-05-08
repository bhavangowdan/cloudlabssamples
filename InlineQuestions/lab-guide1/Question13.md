## Metadata
Question Type : Single Choice

## Question
13. You need to attach a Raw Device Mapping (RDM) for a Microsoft Failover Clustering (MSCS) shared disk between two clustered VMs. Which datastore type is REQUIRED?

## Options
Option 1: NFS datastore
Option 2: VMFS datastore
Option 3: vSAN datastore (HCI mesh)
Option 4: vVols datastore

## Answers
Option 2 : 1

## Correct Answer Feedback
Correct. RDMs require a block-LUN-backed VMFS datastore to host the RDM mapping file. NFS does not present block LUNs; vSAN uses an object store; vVols use VASA-managed virtual volumes.

## Incorrect Answer Feedback
NFS is file-level and cannot expose RDMs. vSAN and vVols handle storage as objects/VVs and do not present raw LUNs to VMs in the RDM sense.

## Tags
VMware
Storage
RDM
Practitioner

## Number of Retries
0
