## Metadata
Question Type : Single Choice

## Question
16. A resource pool "Prod" has CPU shares set to High (8000) and resource pool "Dev" has CPU shares set to Low (2000) at the same level under the cluster. Both pools are CPU-contended. What is the effective CPU allocation ratio between Prod and Dev?

## Options
Option 1: 4:1 (Prod gets 4x Dev)
Option 2: 1:1 (shares only matter when expressed as numeric reservations)
Option 3: 2:1 (Prod gets 2x Dev)
Option 4: Prod gets all CPU until Dev is starving

## Answers
Option 1 : 1

## Correct Answer Feedback
Correct. Shares ratios determine relative entitlement under contention. 8000:2000 = 4:1, so Prod gets four times the contended CPU that Dev gets.

## Incorrect Answer Feedback
Shares are exactly the mechanism for relative allocation under contention; they apply at every parent level. Without contention, both pools get what they ask for; with contention, ratio = shares ratio.

## Tags
VMware
ResourcePool
Shares
Practitioner

## Number of Retries
0
