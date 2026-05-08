## Metadata
Question Type : Single Choice

## Question
21. A McKinsey client wants DB2 z/OS write performance to scale linearly across multiple DB2 members in a Parallel Sysplex. Which DB2 feature DEPENDS on the Coupling Facility to make this possible?

## Options
Option 1: Image Copy
Option 2: Group Buffer Pools (GBPs) for shared cached pages, plus IRLM lock structure for global lock coordination
Option 3: VSAM AIX
Option 4: Online REORG

## Answers
Option 2 : 1

## Correct Answer Feedback
Correct. GBPs in the CF cache database pages shared across members; the IRLM lock structure provides global locking. Without these, write coordination would require disk round-trips and the system would not scale.

## Incorrect Answer Feedback
Image Copy is backup. VSAM AIX is alternate index, unrelated. Online REORG is maintenance.

## Tags
zOS
DB2
CF
Expert

## Number of Retries
0
