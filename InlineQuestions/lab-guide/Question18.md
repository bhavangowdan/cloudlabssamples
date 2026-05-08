## Metadata
Question Type : Single Choice

## Question
18. After a SAN reconfiguration, an AIX 7.x system reports the wrong disk size for an existing hdisk. Which sequence MOST RELIABLY refreshes the device's ODM attributes to match the new SAN-side LUN size?

## Options
Option 1: Reboot the server
Option 2: rmdev -dl hdiskN, then cfgmgr (re-discovers and rebuilds ODM entries; for inflight resize on existing devices use chvg -g <vg> for AIX-native dynamic resize, or extend via chdisk -A on supported MPIO drivers)
Option 3: Manually edit /etc/objrepos files
Option 4: Reinstall AIX

## Answers
Option 2 : 1

## Correct Answer Feedback
Correct. rmdev -dl removes the device from ODM (data on disk untouched), and cfgmgr rediscovers it with current attributes. For LUN size growth on an in-use VG, chvg -g <vg> picks up the new size on PVs in the VG.

## Incorrect Answer Feedback
Reboots are unnecessary and disruptive. ODM files must never be edited manually with a text editor — use odmget/odmchange. Reinstalling AIX is absurd for a SAN-side change.

## Tags
AIX
ODM
SAN
Expert

## Number of Retries
0
