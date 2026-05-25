# Single Static Assignment \(SSA\) form

## Basic idea

An IR in which every variable is assigned exactly once. Joins in control flow are bridged by $\phi$-functions that pick a value based on which predecessor block executed. SSA exposes data-flow directly and makes most optimisations linear.

## Key formulas

- $\phi$-function: $x_3 = \phi(x_1, x_2)$ at a join from blocks $B_1, B_2$.
- Dominance frontier $DF(B)$: nodes where $B$ does *not* strictly dominate but does dominate a predecessor — places where $\phi$-nodes are inserted.
- Cytron et al.'s algorithm: linear in size of dominance frontiers.

