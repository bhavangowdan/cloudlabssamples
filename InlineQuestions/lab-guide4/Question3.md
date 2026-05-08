## Metadata
Question Type : Single Choice

## Question
3. Which z/OS component is responsible for dispatching work and managing CPU resources across address spaces according to performance objectives defined by the installation?

## Options
Option 1: SDSF
Option 2: WLM (Workload Manager) using service classes and goals defined in a service definition
Option 3: JES2
Option 4: TSO/E

## Answers
Option 2 : 1

## Correct Answer Feedback
Correct. WLM matches each unit of work to a service class (which has goals like "response time < 0.5s 90% of the time"), and dispatches CPU + I/O to meet those goals. WLM goals override raw priority — z/OS is goal-driven.

## Incorrect Answer Feedback
SDSF is a UI for SYSLOG / job output. JES2 manages job entry / output. TSO/E is the user shell.

## Tags
zOS
WLM
Practitioner

## Number of Retries
0
