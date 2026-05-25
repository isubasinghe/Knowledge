# Linear Types

## Basic idea

Substructural type system where each value of a linear type is used *exactly once*. Makes resources (file handles, capabilities, qubits) safe to model without a garbage collector and without aliasing bugs.

## Key formulas

- Neither contraction nor weakening: $\Gamma, x:\tau, x:\tau \not\vdash$ and $\Gamma \vdash e \not\Rightarrow \Gamma, x:\tau \vdash e$
- Linear arrow: $\tau \multimap \sigma$ — function consumes argument exactly once.
- Curry-Howard: corresponds to Girard's linear logic.

