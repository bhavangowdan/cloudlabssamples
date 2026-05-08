## Metadata
Question Type : Single Choice

## Question
10. Which VSAM dataset organization supports random access by key, sequential access in key order, and is the typical choice for an indexed customer master file?

## Options
Option 1: ESDS (Entry-Sequenced Dataset)
Option 2: KSDS (Key-Sequenced Dataset)
Option 3: RRDS (Relative Record Dataset)
Option 4: LDS (Linear Dataset)

## Answers
Option 2 : 1

## Correct Answer Feedback
Correct. KSDS is keyed (B-tree-like index over data records), supports random + sequential access, and is the standard for master files. ESDS is entry-sequenced (insertion order, no key). RRDS is by relative record number. LDS is a linear byte stream typically used by DB2 for tablespaces.

## Incorrect Answer Feedback
ESDS, RRDS, LDS each have specific roles but none is the "indexed master file" organization.

## Tags
zOS
VSAM
KSDS
Foundational

## Number of Retries
0
