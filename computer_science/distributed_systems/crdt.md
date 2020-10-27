# CRDT \(Conflict-free Replicated Data Types\)

We can achieve strong eventual consistency through the use of a CRDT.

CRDTs are actually pretty simple. Consider the register **x**. We can perform operations on x such as add\(1\), add\(2\). These operations are commutative and such the order does not matter.

