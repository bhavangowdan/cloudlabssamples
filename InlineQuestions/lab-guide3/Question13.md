## Metadata
Question Type : Single Choice

## Question
13. On Oracle SPARC servers, which LDOM is the special-purpose domain that owns physical I/O hardware (HBAs, network) and presents it virtually to other LDOMs (via vds, vsw, vnet)?

## Options
Option 1: Service Domain (Primary domain by default)
Option 2: Guest Domain
Option 3: Control Domain (manages the hypervisor)
Option 4: Root I/O Domain

## Answers
Option 1 : 1

## Correct Answer Feedback
Correct. The Service Domain owns physical I/O and provides virtual disk/network back-ends to Guest Domains. By default the Primary domain is also the Service Domain and Control Domain. In production, splitting Service Domains for redundancy is common.

## Incorrect Answer Feedback
Guest Domains consume virtual I/O. Control Domain manages the hypervisor (Logical Domains Manager). Root I/O Domain is a sub-pattern that owns specific PCI root complexes.

## Tags
Solaris
LDOM
ServiceDomain
Practitioner

## Number of Retries
0
