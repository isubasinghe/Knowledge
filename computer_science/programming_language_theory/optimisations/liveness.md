# Liveness

## Basic idea

A variable is *live* at a program point if its current value may be used along some path before being overwritten. Backward data-flow analysis: drives register allocation and dead-store elimination.

## Key formulas

- $\mathrm{live\_in}[B]  = \mathrm{use}[B]\ \cup\ (\mathrm{live\_out}[B] \setminus \mathrm{def}[B])$
- $\mathrm{live\_out}[B] = \bigcup_{S \in \mathrm{succ}(B)} \mathrm{live\_in}[S]$
- Lattice: subsets of variables, ordered by $\subseteq$; join is union.

