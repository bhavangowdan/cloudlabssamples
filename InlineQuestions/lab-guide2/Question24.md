## Metadata
Question Type : Single Choice

## Question
24. On IBM Z, which userspace library and kernel mechanism allow zLinux applications to offload AES / RSA / ECC operations to the on-chip CPACF and Crypto Express adapters?

## Options
Option 1: openssl directly bypasses Crypto Express
Option 2: libica + zcrypt kernel module + (optionally) openssl-ibmca / openssl engine + EP11 / CCA host libraries for HSM-mode Crypto Express usage
Option 3: gcrypt only - no Z-specific stack required
Option 4: Linux kernel automatically routes all crypto to CPACF without any library

## Answers
Option 2 : 1

## Correct Answer Feedback
Correct. The s390x crypto stack uses libica for symmetric / hashing offload to CPACF, the zcrypt kernel module for Crypto Express adapters, and an OpenSSL engine (ibmca) to wire the standard OpenSSL APIs to Z hardware. EP11/CCA enable HSM-mode use of Crypto Express.

## Incorrect Answer Feedback
OpenSSL alone does not magically use Z hardware. gcrypt is generic. The kernel exposes hardware crypto via the kernel crypto API, but applications need libica or an engine to opt in.

## Tags
zLinux
Crypto
CPACF
Practitioner

## Number of Retries
0
