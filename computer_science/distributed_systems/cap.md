# CAP \(or more accurately PACELC\) theorem

## Basic idea

Under a network partition, a distributed system must sacrifice either consistency or availability — it cannot keep both. PACELC adds: even when there's no partition, you still trade latency for consistency.

## Key formulas

- CAP: $P \Rightarrow \lnot(C \land A)$ (must drop one of C, A during a partition)
- PACELC: if Partition then choose A or C; Else choose L (latency) or C
- Quorum consistency: $R + W > N$
- PBS: probabilistic bound on staleness for $k$ replicas, $W$ acks: $P(\text{stale}) = f(k, W, \Delta t)$

CAP Theorem asserts that you can only have two of the three, Consistency, Availability or Partition tolerance. However, Partition tolerance must be in place, we do not have the choice to drop Partition tolerance.

PACELC states that in the absence of partitions, you will still have to choose between latency and consistency.

Probabilistic Bounded Staleness \(PBS\) helps us here, it can emperically give a probability to the staleness of our data!.

But interestingly, we dont always have to choose one of CAP, if you drop support for update operations, it is possible to have all three!!

## Resources

* [http://nathanmarz.com/blog/how-to-beat-the-cap-theorem.html](http://nathanmarz.com/blog/how-to-beat-the-cap-theorem.html)
* [https://codahale.com/you-cant-sacrifice-partition-tolerance/](https://codahale.com/you-cant-sacrifice-partition-tolerance/)

