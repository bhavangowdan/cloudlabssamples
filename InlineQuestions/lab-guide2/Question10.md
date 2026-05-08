## Metadata
Question Type : Multiple Choice

## Question
10. When configuring multipath for FCP-attached storage on zLinux, which TWO device file patterns represent the underlying paths BEFORE multipathd aggregates them? (Select two)

## Options
Option 1: /dev/sd* (e.g., /dev/sda, /dev/sdb)
Option 2: /dev/dasd* (e.g., /dev/dasda)
Option 3: /dev/disk/by-path/ccw-* paths
Option 4: /dev/disk/by-path/ccw-*-fc-* paths
Option 5: /dev/mapper/mpath*

## Answers
Option 1 : 1
Option 4 : 1

## Correct Answer Feedback
Correct. FCP LUNs appear as /dev/sd* devices (Option 1) addressable via /dev/disk/by-path/ccw-X.X.XXXX-fc-WWPN-lun-N (Option 4). multipathd then aggregates them into /dev/mapper/mpath* devices.

## Incorrect Answer Feedback
/dev/dasd* is for ECKD DASD, not FCP. /dev/disk/by-path/ccw-* (without -fc-) is for ECKD. /dev/mapper/mpath* is the post-aggregation device, not an underlying path.

## Tags
zLinux
Storage
Multipath
Practitioner

## Number of Retries
0
