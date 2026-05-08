## Metadata
Question Type : Single Choice

## Question
16. On Solaris 11, which command applies all available updates from configured publishers, automatically creating a new boot environment?

## Options
Option 1: pkg update
Option 2: pkg install --all
Option 3: yum update
Option 4: smpatch update

## Answers
Option 1 : 1

## Correct Answer Feedback
Correct. pkg update applies all available package updates from publishers; if the update affects boot-time or kernel components, IPS automatically creates a new BE that you boot into for the change to take effect (zero-downtime fallback via beadm activate).

## Incorrect Answer Feedback
pkg install --all is not the standard form. yum is Linux. smpatch is the legacy Solaris 10 patch tool.

## Tags
Solaris
IPS
pkg
Practitioner

## Number of Retries
0
