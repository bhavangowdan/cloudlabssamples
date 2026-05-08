## Metadata
Question Type : Single Choice

## Question
18. What does FTT (Failures To Tolerate) = 1 mean for a vSAN object on a hybrid cluster with a RAID-1 storage policy?

## Options
Option 1: vSAN keeps two copies of the object on two different hosts; the cluster can tolerate 1 host or disk failure without data loss
Option 2: vSAN keeps one copy of the object; FTT=1 disables redundancy
Option 3: vSAN keeps three copies; FTT counts mirrors-1
Option 4: FTT only applies to all-flash clusters, not hybrid

## Answers
Option 1 : 1

## Correct Answer Feedback
Correct. FTT=1 with RAID-1 = mirror across two hosts plus a witness component. The cluster survives loss of one fault domain (typically one host) without data loss.

## Incorrect Answer Feedback
FTT=1 explicitly enables one level of redundancy. FTT does not equal mirror_count - 1. FTT is a vSAN policy attribute that applies to both hybrid and all-flash.

## Tags
VMware
vSAN
FTT
Foundational

## Number of Retries
0
