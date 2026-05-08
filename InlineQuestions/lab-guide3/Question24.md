## Metadata
Question Type : Single Choice

## Question
24. A McKinsey client running Solaris 10 SPARC custom-app workloads wants to migrate to RHEL 8 on x86. The vendor has provided RHEL 8 binaries. What is a KEY architectural risk to flag during assessment?

## Options
Option 1: SPARC is little-endian, x86 is big-endian, so binary data files are incompatible
Option 2: SPARC is big-endian, x86 is little-endian, so any binary data file (e.g., custom on-disk records, certain checkpoint formats) may need byte-swap conversion or re-creation on the target
Option 3: SPARC and x86 use identical ABIs so binaries port directly
Option 4: ZFS is unsupported on Linux so all data is lost

## Answers
Option 2 : 1

## Correct Answer Feedback
Correct. SPARC is big-endian; x86 is little-endian. Binary on-disk data (custom record formats, structured logs, application-specific dumps) may require re-creation or explicit byte-swap. Standard formats (CSV, JSON, properly-versioned DB) are not affected.

## Incorrect Answer Feedback
The endian directions are swapped (Option 1 reverses them). ABIs are different (Option 3). ZFS-on-Linux exists, so data movement is feasible (Option 4 is wrong).

## Tags
Solaris
Modernization
Endian
Practitioner

## Number of Retries
0
