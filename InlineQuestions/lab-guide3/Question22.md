## Metadata
Question Type : Single Choice

## Question
22. What is the purpose of beadm in Solaris 11?

## Options
Option 1: To manage boot environments (BEs) — clone the active BE before risky changes (e.g., kernel patch), boot into the new BE, fall back to the previous BE if needed
Option 2: To manage boot loaders
Option 3: To manage backups via NetBackup
Option 4: To manage the eeprom OBP

## Answers
Option 1 : 1

## Correct Answer Feedback
Correct. beadm (boot environment admin) leverages ZFS snapshots/clones to create alternate Solaris instances on the same root pool. Combined with IPS, this enables zero-downtime rollback after pkg update.

## Incorrect Answer Feedback
Boot loaders are managed by bootadm / installgrub. NetBackup is third-party. eeprom OBP is the SPARC OpenBoot tool.

## Tags
Solaris
beadm
BootEnvironment
Practitioner

## Number of Retries
0
