## Metadata
Question Type : Single Choice

## Question
15. On a zLinux RHEL 8 system, which Linux network interface name typically corresponds to a HiperSockets device after qeth driver binding?

## Options
Option 1: eth0 (renamed by udev to enXXXX)
Option 2: hsi0
Option 3: hsn0
Option 4: enp0s1

## Answers
Option 2 : 1

## Correct Answer Feedback
Correct. By convention, qeth-driven HiperSockets devices appear as hsiN (HiperSockets Interface) under predictable network naming on RHEL/SLES on Z. OSA-Express uses encXXXX.

## Incorrect Answer Feedback
hsn0 and enp0s1 are not standard Z naming. eth0 is the legacy alias pre-systemd predictable naming.

## Tags
zLinux
Networking
HiperSockets
Practitioner

## Number of Retries
0
