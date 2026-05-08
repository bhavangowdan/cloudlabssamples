## Metadata
Question Type : Single Choice

## Question
17. Which encoding does Linux on IBM Z use for files on its native filesystem (e.g., ext4, XFS)?

## Options
Option 1: EBCDIC (because it runs on a mainframe)
Option 2: UTF-8 / ASCII (zLinux is a standard Linux userland - it is little-endian-aware on s390x but uses Linux-native encodings)
Option 3: Always UTF-16
Option 4: Whatever encoding was set in the LPAR profile

## Answers
Option 2 : 1

## Correct Answer Feedback
Correct. zLinux uses standard Linux encodings (UTF-8 by default, ASCII for legacy ASCII text). EBCDIC is a z/OS / VM/CMS concern. When zLinux exchanges data with z/OS via FTP / Connect:Direct / pipes, conversion is required (typically iconv).

## Incorrect Answer Feedback
EBCDIC is not the zLinux native encoding — that is a frequent confusion among admins new to Z. UTF-16 is for specific applications. LPAR profile sets hardware, not user-space encoding.

## Tags
zLinux
EBCDIC
Encoding
Practitioner

## Number of Retries
0
