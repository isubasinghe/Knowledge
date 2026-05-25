# CRDT \(Conflict-free Replicated Data Types\)

## Basic idea

Data types whose concurrent updates *always* merge deterministically without coordination. Achieved by making operations commutative (op-based) or by defining a join over a semilattice of states (state-based).

## Key formulas

- State-based merge must form a join-semilattice: $a \sqcup b$ exists, is commutative, associative, idempotent.
- Op-based: all concurrent ops must commute: $op_i \circ op_j = op_j \circ op_i$.
- Convergence: replicas applying the same set of updates (in any order) reach equal states — *strong eventual consistency*.

We can achieve strong eventual consistency through the use of a CRDT.

CRDTs are actually pretty simple. Consider the register **x**. We can perform operations on x such as add\(1\), add\(2\). These operations are commutative and such the order does not matter.

