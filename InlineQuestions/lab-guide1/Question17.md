## Metadata
Question Type : Single Choice

## Question
17. You set a 4 GHz CPU reservation on a resource pool that contains 50 VMs. None of the individual VMs have their own reservations. What does this guarantee under contention?

## Options
Option 1: Each of the 50 VMs gets a guaranteed 4 GHz of CPU
Option 2: The resource pool collectively gets a guaranteed 4 GHz, distributed among its VMs based on their shares and demand
Option 3: Reservations cannot be set at the resource pool level — only at the VM level
Option 4: Each VM gets 4 GHz / 50 = 80 MHz guaranteed

## Answers
Option 2 : 1

## Correct Answer Feedback
Correct. A pool-level reservation guarantees the pool's aggregate entitlement. Inside the pool, distribution between VMs follows their shares and active demand — VMware does not statically subdivide the reservation per VM.

## Incorrect Answer Feedback
Reservation is a pool-level guarantee, not a per-VM multiplier. Reservations are valid at pool level. Distribution is dynamic, not equal-split.

## Tags
VMware
ResourcePool
Reservation
Expert

## Number of Retries
0
