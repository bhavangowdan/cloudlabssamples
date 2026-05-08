## Metadata
Question Type : Single Choice

## Question
5. A Solaris 11 service has been started, then died, and is now in the "maintenance" state. Which command sequence diagnoses the cause and clears the state?

## Options
Option 1: svcs -xv to see why; review the service log file shown in the output; fix the underlying problem; svcadm clear <fmri>
Option 2: svcs -a; rm -rf /var/svc; reboot
Option 3: pkg update; rebuild the manifest
Option 4: svccfg delete <fmri>; svccfg import <fmri>

## Answers
Option 1 : 1

## Correct Answer Feedback
Correct. svcs -xv flags broken services and points to the relevant log file under /var/svc/log/. Fix the issue, then svcadm clear to bring the service back online.

## Incorrect Answer Feedback
Removing /var/svc destroys the SMF repository. pkg update is unrelated. Deleting and re-importing the manifest is overkill (and loses customization).

## Tags
Solaris
SMF
Troubleshooting
Practitioner

## Number of Retries
0
