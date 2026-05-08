## Metadata
Question Type : Single Choice

## Question
14. Which AIX LVM construct holds the metadata describing all PVs, LVs, and PPs of a Volume Group?

## Options
Option 1: ODM only
Option 2: VGDA (Volume Group Descriptor Area) on each PV
Option 3: /etc/fstab
Option 4: smit.log

## Answers
Option 2 : 1

## Correct Answer Feedback
Correct. VGDA is replicated on each PV in the VG and holds the LVM metadata. AIX uses VGDA quorum (>50% reachable) to keep the VG online. ODM also caches device info but is not the source of truth across hosts.

## Incorrect Answer Feedback
ODM is the per-host configuration database. /etc/fstab is /etc/filesystems on AIX (and is mount config, not LVM metadata). smit.log is just a log.

## Tags
AIX
LVM
VGDA
Foundational

## Number of Retries
0
