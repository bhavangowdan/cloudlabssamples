## Metadata
Question Type : Single Choice

## Question
14. A McKinsey client wants live migration of a Solaris LDOM from one SPARC server to another with no application downtime. Which feature accomplishes this?

## Options
Option 1: ldm migrate-domain (Live Domain Migration)
Option 2: Solaris vMotion
Option 3: zoneadm move
Option 4: zfs send

## Answers
Option 1 : 1

## Correct Answer Feedback
Correct. Oracle VM Server for SPARC (LDoms) supports Live Domain Migration via `ldm migrate-domain`, with shared storage (FC SAN) and compatible processor / firmware levels.

## Incorrect Answer Feedback
"Solaris vMotion" is not a thing. zoneadm move offline-relocates a zone's path, not a live migration. zfs send replicates filesystems.

## Tags
Solaris
LDOM
LiveMigration
Practitioner

## Number of Retries
0
