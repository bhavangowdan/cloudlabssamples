## Metadata
Question Type : Single Choice

## Question
4. On Solaris 11, which command places an SMF service in the maintenance state for repair?

## Options
Option 1: svcadm clear <fmri>
Option 2: svcadm mark maintenance <fmri>
Option 3: svcs -p <fmri>
Option 4: svccfg validate <fmri>

## Answers
Option 2 : 1

## Correct Answer Feedback
Correct. svcadm mark maintenance forces a service to maintenance state, halting dependent services. svcadm clear is the inverse — it transitions a service OUT of maintenance after the underlying issue is resolved.

## Incorrect Answer Feedback
svcadm clear undoes maintenance state. svcs -p shows processes. svccfg validate validates the manifest.

## Tags
Solaris
SMF
Practitioner

## Number of Retries
0
