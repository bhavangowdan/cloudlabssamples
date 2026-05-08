## Metadata
Question Type : Single Choice

## Question
8. A McKinsey client has dual-VIOS (VIOS1 + VIOS2) on a POWER10 frame. VIOS1 is rebooted for patching while client LPARs are running. The client LPARs use NPIV with multipathing. What is the EXPECTED behavior?

## Options
Option 1: All client LPARs hang because the SAN-side WWPN moves to VIOS2
Option 2: MPIO on the client LPAR detects path-down on the VIOS1-routed paths, fails over to VIOS2-routed paths, and I/O continues without application impact
Option 3: VIOS1 reboot is blocked by HMC if any client LPAR is running
Option 4: All client filesystems are remounted read-only

## Answers
Option 2 : 1

## Correct Answer Feedback
Correct. With dual-VIOS NPIV + MPIO, the SAN sees two virtual WWPNs per client (one through each VIOS). When VIOS1 reboots, MPIO on the client marks those paths as Failed and continues over VIOS2's paths. This is exactly why dual-VIOS is the production standard.

## Incorrect Answer Feedback
The WWPN is per-vfchost, not migrated. HMC does not block VIOS reboots — that is the operator's responsibility. Filesystems do not auto-remount RO unless lvm quorum is lost (which dual-VIOS prevents).

## Tags
AIX
VIOS
NPIV
MPIO
Expert

## Number of Retries
0
