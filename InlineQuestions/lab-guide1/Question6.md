## Metadata
Question Type : Single Choice

## Question
6. What is the recommended minimum dedicated network bandwidth (per VMkernel adapter) for vMotion in vSphere 7.x?

## Options
Option 1: 100 Mbps
Option 2: 1 Gbps
Option 3: 10 Gbps
Option 4: 25 Gbps

## Answers
Option 3 : 1

## Correct Answer Feedback
Correct. VMware recommends 10 GbE (or higher) for vMotion in vSphere 6.7+ to enable encrypted vMotion, multi-NIC vMotion, and large-memory VM migrations within reasonable time.

## Incorrect Answer Feedback
1 GbE works for small lab use but is below the supported recommendation for production in vSphere 7.x. 25 GbE exceeds the minimum.

## Tags
VMware
vMotion
Networking
Foundational

## Number of Retries
0
