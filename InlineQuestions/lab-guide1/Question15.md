## Metadata
Question Type : Text Input

## Question
15. A virtual machine has 14 snapshots stacked one after another (a deep snapshot tree) that haven’t been cleaned up for 60 days. When you try to move this VM to another datastore using Storage vMotion, the migration fails halfway. Explain: (a) What is the most likely reason for this failure? (b) In what order should you fix the issue? only answer in 1 word 

## Options
N/A

## Answers
^(?i)(snapshots|consolidation|depth|chain|failure|corruption|cleanup|remediation|storage|datastore|migration|hierarchy|limit|error|disk)$

## Correct Answer Feedback
Long snapshot chains create cumulative delta files (sesparse / -delta.vmdk) that grow during the migration as the VM keeps writing. Likely root cause: datastore filled up mid-copy, or a consolidation lock conflict / I/O timeout. Remediation order: (1) cancel the Storage vMotion, (2) quiesce VM I/O if possible, (3) consolidate snapshots first via Snapshot Manager > Consolidate, (4) confirm delta files are gone via the datastore browser, (5) retry Storage vMotion. Never delete delta files manually from the datastore.

## Incorrect Answer Feedback
A common wrong answer is to delete delta VMDKs manually to "free space" — this corrupts the VM. Always consolidate via vCenter (or vmkfstools / VMware Support if consolidation itself fails).

## Tags
VMware
Snapshots
Troubleshooting
Practitioner

## Number of Retries
0
