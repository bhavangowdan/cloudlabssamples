## Metadata
Question Type : Single Choice

## Question
1. Which vCenter Server component is responsible for storing the inventory hierarchy and configuration data for managed ESXi hosts and virtual machines?

## Options
Option 1: vpxd (VPX Daemon)
Option 2: vCenter Server Appliance Database (VCDB / embedded PostgreSQL)
Option 3: ESXi hostd
Option 4: vSphere Client

## Answers
Option 2 : 1

## Correct Answer Feedback
Correct. The VCDB (embedded PostgreSQL on the vCenter Server Appliance) persists inventory, configuration, performance metrics, and tasks/events. It is the source of truth for vCenter state.

## Incorrect Answer Feedback
vpxd is the management process that talks to the database, hostd runs on each ESXi host (not vCenter), and the vSphere Client is only a UI. The persistence layer is the VCDB.

## Tags
VMware
vSphere
Architecture
Foundational

## Number of Retries
0
