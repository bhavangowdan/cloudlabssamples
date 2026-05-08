## Metadata
Question Type : Single Choice

## Question
14. Which statement about HiperSockets is MOST accurate?

## Options
Option 1: HiperSockets is a 100 Gbps Ethernet adapter that connects the mainframe to external networks
Option 2: HiperSockets is a memory-based, in-CPC TCP/IP network connecting LPARs and z/VM guests within the same physical machine with no external cabling
Option 3: HiperSockets is a SAN protocol used between the mainframe and IBM DS8000 storage
Option 4: HiperSockets is a workload-management feature that prioritizes high-priority TCP connections

## Answers
Option 2 : 1

## Correct Answer Feedback
Correct. HiperSockets uses internal LPAR-to-LPAR memory copies for TCP/IP traffic, with near-zero latency and no physical NIC involvement. Frequent use case: z/OS LPAR talking to a zLinux LPAR on the same CPC.

## Incorrect Answer Feedback
External Ethernet uses OSA-Express. SAN to DS8000 uses FICON / FCP. Connection prioritization is a WLM / network-policy concern, not HiperSockets.

## Tags
zLinux
Networking
HiperSockets
Practitioner

## Number of Retries
0
