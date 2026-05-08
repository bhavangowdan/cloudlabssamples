## Metadata
Question Type : Multiple Choice

## Question
11. Which TWO statements about a PDSE compared to a classic PDS are correct? (Select two)

## Options
Option 1: PDSE reuses space when members are deleted; PDS does not (requires compress)
Option 2: PDSE supports more than 65,535 directory blocks
Option 3: PDS and PDSE are interchangeable — same underlying structure
Option 4: PDSE can hold load modules but PDS cannot hold any executables
Option 5: Both PDS and PDSE require compression with IEBCOPY periodically to reclaim deleted-member space

## Answers
Option 1 : 1
Option 2 : 1

## Correct Answer Feedback
Correct. PDSE auto-reclaims space on member delete (Option 1) and has dynamic directory (Option 2). PDS and PDSE are NOT the same internally (Option 3 wrong). Both PDS and PDSE can hold executables — PDS holds load modules, PDSE holds program objects (Option 4 wrong). Only PDS requires compress; PDSE does not (Option 5 wrong).

## Incorrect Answer Feedback
The clearest gotcha is treating PDS and PDSE as the same (they share an external API but differ structurally and behaviorally).

## Tags
zOS
Datasets
PDSE
Practitioner

## Number of Retries
0
