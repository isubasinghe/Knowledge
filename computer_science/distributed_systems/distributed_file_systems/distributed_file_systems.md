# Distributed File Systems

## Basic idea

File systems whose data and metadata are spread across many networked machines. The hard part is that each "fix" introduces the next problem — sharding fixes performance but adds faults, replication fixes faults but adds inconsistency.

## Key facts

- Loop of tradeoffs: performance → sharding → faults → replication → inconsistency → low performance.
- Probabilistic Bounded Staleness (PBS) gives a quantifiable handle on the last step.
- Replication factor $r$ tolerates $r-1$ node failures.

## Why are distributed file systems hard?
Distributed systems need performance

* Performance `fixedBy` Sharding
* Sharding `fixedBy` Faults
* Faults `fixedBy` Tolerance 
* Tolerance `fixedBy` Replication 
* Replication `fixedBy` Inconsistencies
* Inconsistencies `fixedBy` Low performance
* Low performance `fixedBy` mitigate with Probabilistic Bounded Staleness 

