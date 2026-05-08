## Metadata
Question Type : Single Choice

## Question
28. Which is the BEST description of GRS star configuration on z/OS?

## Options
Option 1: A failed configuration topology
Option 2: A Global Resource Serialization configuration where all systems are connected to a CF-resident lock structure (star topology); replaces the older RING topology and is the recommended Parallel Sysplex GRS configuration
Option 3: A new sysplex name introduced in z/OS 2.5
Option 4: A backup tool for DASD

## Answers
Option 2 : 1

## Correct Answer Feedback
Correct. GRS star is the recommended GRS topology for Parallel Sysplex — all members coordinate global ENQ/DEQ via a CF lock structure, with star semantics (no token passing required). Older RING topology is in maintenance only.

## Incorrect Answer Feedback
GRS star is a current, supported topology — not a failure or a new sysplex name.

## Tags
zOS
Sysplex
GRS
Expert

## Number of Retries
0
