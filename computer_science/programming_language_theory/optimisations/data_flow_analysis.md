# Data Flow Analysis

## Basic idea

Compute, for every program point, a conservative summary of all execution paths that could reach it. Framed as a fixpoint over a lattice: each instruction has a transfer function, joins use the lattice meet/join.

## Key formulas

- Forward: $\mathrm{OUT}[B] = f_B(\mathrm{IN}[B])$, $\mathrm{IN}[B] = \bigsqcup_{P \in \mathrm{pred}(B)} \mathrm{OUT}[P]$
- Backward: $\mathrm{IN}[B] = f_B(\mathrm{OUT}[B])$, $\mathrm{OUT}[B] = \bigsqcup_{S \in \mathrm{succ}(B)} \mathrm{IN}[S]$
- Termination guaranteed for monotone $f$ on a finite-height lattice (Tarski).
- Examples: reaching definitions, live variables, available expressions, very-busy expressions.

