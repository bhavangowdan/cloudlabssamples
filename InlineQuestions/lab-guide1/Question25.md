## Metadata
Question Type : Text Input 

## Question
25.You have a 3-node vSAN cluster (each host has 1 cache disk + 2 capacity disks). You notice that 40% of VM objects show reduced redundancy. The health check reports that on host esx-02, one capacity disk is showing high latency and read errors.
Explain:
(a) How would you diagnose this issue step by step?
(b) What actions would you take to fix it?
(c) What risks to data placement exist while you are fixing the problem? ONLY answer in 1 word

## Options
N/A

## Answers
^(?i)(diagnostic|remediation|risk|latency|errors|capacity|disk|host|redundancy|health|placement|migration|failure|cluster|storage)$

## Correct Answer Feedback
Diagnostic order: (1) confirm disk health via esxcli vsan storage list and vendor SMART tools — read errors + latency are pre-failure; (2) check vSAN object health (RVC vsan.check_state) — "reduced redundancy" means components on the failing disk are still serving I/O but FTT is degraded; (3) verify cluster has rebuild capacity (cluster < 70% used). Remediation: place the suspect disk in Maintenance Mode with "Full data migration" so vSAN evacuates components to remaining capacity disks on healthy hosts, then replace the disk and re-add to the disk group. Data-placement risk: with only 3 nodes and FTT=1, evacuating one disk in a 3-fault-domain cluster leaves zero rebuild headroom — any second failure during rebuild can lead to data loss. Mitigations: take backups, schedule the operation in a maintenance window, and consider temporarily adding a 4th host if available.

## Incorrect Answer Feedback
A common wrong path is hot-pulling the failing disk before evacuation, which forces emergency rebuild and risks data loss with only 3 fault domains. Always evacuate first.

## Tags
VMware
vSAN
Troubleshooting
Expert

## Number of Retries
0
