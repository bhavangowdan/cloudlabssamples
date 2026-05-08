## Metadata
Question Type : Single Choice

## Question
18. On a zLinux RHEL 8 system attached to FCP storage, which utility produces a dump that is written to a dedicated FCP-attached dump device for offline analysis?

## Options
Option 1: kdump on a regular crashkernel
Option 2: zfcpdump - a special-purpose dump tool that runs from a small standalone Linux image and dumps to an FCP device
Option 3: makedumpfile only
Option 4: vmcore-write

## Answers
Option 2 : 1

## Correct Answer Feedback
Correct. zfcpdump (also called the "zfcpdump tool") is a tiny Linux dump environment that boots from a designated FCP dump partition and writes the system memory of a crashed Linux instance for later analysis with crash/lcrash.

## Incorrect Answer Feedback
Standard kdump works on Z too but boots a kdump kernel into reserved memory. zfcpdump is the FCP-targeted variant. makedumpfile compresses an existing dump; vmcore-write is not the standard tool.

## Tags
zLinux
Dump
zfcpdump
Practitioner

## Number of Retries
0
