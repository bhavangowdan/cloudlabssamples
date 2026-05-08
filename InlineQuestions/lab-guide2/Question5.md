## Metadata
Question Type : Multiple Choice

## Question
5. Which TWO of the following are valid mechanisms by which z/VM enables high-density Linux virtualization? (Select two)

## Options
Option 1: NSS (Named Saved Segments) - shared kernel image across many guests
Option 2: DCSS (Discontiguous Saved Segments) - shared read-only memory segments across guests
Option 3: vMotion across z/VM hosts
Option 4: Direct hardware passthrough of every PCI card to every guest
Option 5: Hyper-V Replica service

## Answers
Option 1 : 1
Option 2 : 1

## Correct Answer Feedback
Correct. NSS lets multiple guests share an in-memory copy of the kernel + initramfs (Option 1). DCSS lets guests share read-only memory segments such as application libraries (Option 2). Both are core to z/VM's ability to run hundreds of Linux guests on one LPAR.

## Incorrect Answer Feedback
vMotion is a VMware feature; z/VM has its own Live Guest Relocation (LGR) within an SSI cluster. PCI passthrough is not the dense-virtualization mechanism. Hyper-V Replica is a Microsoft feature.

## Tags
zLinux
zVM
NSS
Practitioner

## Number of Retries
0
