## Metadata
Question Type : Single Choice

## Question
4. On a POWER10 frame with PowerVM Enterprise, you create an LPAR with "uncapped" processing-unit mode and weight=128. What does this configuration imply at runtime?

## Options
Option 1: The LPAR's CPU usage is fixed at the entitled processing units; it never receives more
Option 2: The LPAR can consume CPU above its entitled processing units when the shared pool has spare capacity, with priority relative to other uncapped LPARs determined by weight
Option 3: The LPAR is dedicated and cannot share CPU with any other LPAR
Option 4: The LPAR runs only when no other LPARs need CPU

## Answers
Option 2 : 1

## Correct Answer Feedback
Correct. Uncapped LPARs can borrow unused CPU from the shared processor pool above their entitlement, with weight (1-255) determining priority among competing uncapped LPARs.

## Incorrect Answer Feedback
Capped mode fixes usage at entitlement. Dedicated mode does not share. Uncapped is the opposite of "lowest priority" — it competes by weight.

## Tags
AIX
LPAR
Uncapped
Practitioner

## Number of Retries
0
