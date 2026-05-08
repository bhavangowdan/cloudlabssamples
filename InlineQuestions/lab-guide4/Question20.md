## Metadata
Question Type : Single Choice

## Question
20. What is DB2 z/OS Data Sharing?

## Options
Option 1: A backup-and-restore facility
Option 2: A configuration where multiple DB2 members across multiple z/OS images share a single set of databases (tablespaces, indexes) on shared DASD via the Coupling Facility for locking and buffer pool coherency
Option 3: A read-only replication tool to copy DB2 to Linux
Option 4: A row-level security feature

## Answers
Option 2 : 1

## Correct Answer Feedback
Correct. DB2 Data Sharing is the foundation of horizontal scale and HA for DB2 z/OS in a Parallel Sysplex. Members coordinate via the CF (IRLM lock structure, GBP cache structures), share DASD, and present a single logical DB to applications.

## Incorrect Answer Feedback
Backup is BACKUP SYSTEM / image copy. Cross-platform replication is IIDR / Q-replication. RLS is a separate authorization feature.

## Tags
zOS
DB2
DataSharing
Practitioner

## Number of Retries
0
