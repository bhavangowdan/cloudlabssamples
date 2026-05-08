## Metadata
Question Type : Single Choice

## Question
22. Which of the following is FALSE regarding the management plane in Azure VMware Solution (AVS)?

## Options
Option 1: Customer has full root access to ESXi hosts via SSH
Option 2: vCenter Server is managed by Microsoft but customer has cloudadmin role
Option 3: NSX-T Manager is included and customer can configure segments and gateways
Option 4: HCX is available as an add-on for migration

## Answers
Option 1 : 1

## Correct Answer Feedback
Correct (this option is FALSE). AVS is a managed service; Microsoft retains root on the ESXi hosts and the underlying SDDC. Customers operate at the cloudadmin role on vCenter, configure NSX-T (with appropriate constraints), and license HCX for migration — but never get host root.

## Incorrect Answer Feedback
The customer-facing roles are cloudadmin (not root), NSX-T Manager access is exposed, and HCX is included/add-on. Root SSH on ESXi is reserved to Microsoft.

## Tags
VMware
AVS
Security
Expert

## Number of Retries
0
