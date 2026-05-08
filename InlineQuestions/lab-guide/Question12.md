## Metadata
Question Type : Single Choice

## Question
12. On AIX 7.x, which command extends a JFS2 filesystem named /data online without unmounting?

## Options
Option 1: chfs -a size=+10G /data
Option 2: resize2fs /dev/datalv 100G
Option 3: xfs_growfs /data
Option 4: extendfs -y /data

## Answers
Option 1 : 1

## Correct Answer Feedback
Correct. chfs -a size=+10G /data extends the filesystem online by 10 GB. The underlying LV is grown automatically if needed (or use chlv first, then chfs).

## Incorrect Answer Feedback
resize2fs is ext2/3/4. xfs_growfs is XFS. extendfs is the older AIX command and -y is not its syntax.

## Tags
AIX
JFS2
chfs
Practitioner

## Number of Retries
0
