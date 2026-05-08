## Metadata
Question Type : Single Choice

## Question
21. On Solaris 11, which command creates a virtual NIC (VNIC) bound to an etherstub (a virtual switch) for connecting zones without using physical interfaces?

## Options
Option 1: dladm create-vnic -l <etherstub> <vnic-name>
Option 2: ifconfig <vnic> create
Option 3: ipadm create-addr
Option 4: zonecfg add net

## Answers
Option 1 : 1

## Correct Answer Feedback
Correct. The Crossbow network virtualization stack provides etherstubs (virtual switches) and VNICs created via dladm create-vnic -l <etherstub or physical link>. Zones consume these via zonecfg add anet (automatic VNIC) or static net resources.

## Incorrect Answer Feedback
ifconfig is legacy. ipadm manages IP addresses on a link, not the link itself. zonecfg add net references an existing data link.

## Tags
Solaris
Crossbow
VNIC
Practitioner

## Number of Retries
0
