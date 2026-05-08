## Metadata
Question Type : Single Choice

## Question
12. Which Solaris 11 command creates and configures a new non-kernel zone interactively?

## Options
Option 1: zoneadm create
Option 2: zonecfg -z <zonename>
Option 3: zlogin <zonename>
Option 4: zonename create <zonename>

## Answers
Option 2 : 1

## Correct Answer Feedback
Correct. zonecfg -z <zonename> opens an interactive (or scriptable) configuration session to define zone properties (zonepath, network, resource pools). zoneadm install / boot / list comes after.

## Incorrect Answer Feedback
zoneadm install/boot operates on a configured zone. zlogin connects to an already-running zone. zonename is a query command.

## Tags
Solaris
Zones
zonecfg
Practitioner

## Number of Retries
0
