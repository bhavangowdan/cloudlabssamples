## Metadata
Question Type : Single Choice

## Question
23. A legacy z/OS COBOL batch workload is being modernized. The customer wants to keep the COBOL code as-is but move execution off z/OS to reduce MIPS. Which target environment KEEPS the workload on IBM Z hardware while exiting z/OS billing?

## Options
Option 1: zLinux on IFLs running an open-source or third-party COBOL runtime (e.g., GnuCOBOL, Micro Focus Visual COBOL for Linux)
Option 2: AWS EC2 with WebSphere
Option 3: Azure Functions with C#
Option 4: x86 RHEL with WebSphere Liberty

## Answers
Option 1 : 1

## Correct Answer Feedback
Correct. zLinux on IFLs is a partial modernization path: workloads stay on Z hardware (RAS, location, security posture preserved) but execute on IFLs which are not billed under z/OS MLC pricing. COBOL is recompiled with a Linux-native compiler.

## Incorrect Answer Feedback
EC2, Azure Functions, and x86 RHEL all move OFF Z hardware entirely. They are full-replatform options, not the "keep on Z, exit z/OS" pattern this question asks about.

## Tags
zLinux
Modernization
COBOL
Practitioner

## Number of Retries
0
