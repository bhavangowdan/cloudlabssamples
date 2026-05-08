## Metadata
Question Type : Single Choice

## Question
25. Which IBM Z security feature provides "pervasive encryption" - encryption of data at rest at the dataset / volume level with minimal application change?

## Options
Option 1: AES-NI on x86 with kernel transparency
Option 2: dm-crypt / LUKS keyed by master keys held in Crypto Express HSM via secure-key support, plus kernel integration so the encryption is transparent to applications
Option 3: TLS 1.3 termination at the OSA-Express adapter
Option 4: SE Linux mandatory access control

## Answers
Option 2 : 1

## Correct Answer Feedback
Correct. Pervasive encryption on Z uses dm-crypt (and on z/OS, dataset encryption) with master keys protected by Crypto Express HSMs in secure-key mode. The volume key is wrapped under the HSM master key, applications stay unchanged, and key extraction from the HSM is prevented by hardware.

## Incorrect Answer Feedback
AES-NI is x86. TLS at OSA is in-flight, not at-rest. SELinux is access control, not encryption.

## Tags
zLinux
Crypto
PervasiveEncryption
Expert

## Number of Retries
0
