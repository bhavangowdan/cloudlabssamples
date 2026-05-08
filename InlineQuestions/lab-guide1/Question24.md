## Metadata
Question Type : Single Choice

## Question
24. A VM stops responding to the guest OS but vCenter still shows it as Powered On. The vSphere Client "Open Console" hangs and you cannot RDP/SSH to the guest. Which is the most appropriate FIRST troubleshooting action?

## Options
Option 1: Power off the host running the VM to recover
Option 2: From the host, list the running vmx process for the VM (esxcli vm process list) and check vmware.log for the VM, then attempt a guest-OS-level reset via "Reset Guest OS" or "Power Off VM" from vCenter
Option 3: Delete and recreate the VM
Option 4: Roll back the VM to a 6-month-old snapshot

## Answers
Option 2 : 1

## Correct Answer Feedback
Correct. Standard diagnostic flow: confirm the vmx process is alive on the host, inspect vmware.log for storage timeouts / guest crashes, then issue a controlled reset/power-off from vCenter. Powering off the host is reserved for hung host scenarios.

## Incorrect Answer Feedback
Powering off the host affects every VM on that host. Recreating the VM destroys data. Rolling back to old snapshots is destructive and unrelated to a hung guest.

## Tags
VMware
Troubleshooting
Practitioner

## Number of Retries
0
