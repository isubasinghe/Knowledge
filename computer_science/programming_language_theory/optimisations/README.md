# optimisations

## Basic idea

Semantics-preserving program transformations that make code run faster or smaller. Classical optimisations operate on basic blocks or control-flow graphs and are framed as data-flow analyses.

## Key facts

- Data-flow analyses solve fixpoints over a lattice on the CFG.
- Common: constant propagation, dead-code elimination, CSE, loop-invariant code motion, inlining, peephole.
- SSA form makes most of these one-pass and local.

