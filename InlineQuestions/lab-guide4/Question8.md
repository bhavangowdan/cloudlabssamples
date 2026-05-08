## Metadata
Question Type : Single Choice

## Question
8. A batch job ABENDs with S0C7 in step 3 of a 5-step JCL. Step 4 has COND=(4,LT,STEP02). What happens to step 4?

## Options
Option 1: Step 4 always runs because COND on step 4 is not tied to step 3
Option 2: Step 4 is bypassed because, by default, an abend in any preceding step bypasses subsequent steps unless they have COND=EVEN or COND=ONLY — independent of any other COND test
Option 3: Step 4 runs only if step 3 also abends
Option 4: COND=(4,LT,STEP02) cancels step 4 unconditionally

## Answers
Option 2 : 1

## Correct Answer Feedback
Correct. When any prior step abends, JES bypasses subsequent steps by default. To run a step after an abend, use COND=EVEN; to run a step ONLY after an abend, use COND=ONLY. The numeric COND test (4,LT,STEP02) is unrelated to the abend-bypass.

## Incorrect Answer Feedback
COND=(4,LT,STEP02) tests the return code of STEP02; it does not override abend-bypass behavior. The other interpretations misread the COND semantics.

## Tags
zOS
JCL
COND
ABEND
Expert

## Number of Retries
0
