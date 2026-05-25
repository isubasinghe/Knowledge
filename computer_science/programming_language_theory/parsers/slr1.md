# SLR\(1\) parser

## Basic idea

Simple LR(1): an LR(0) automaton augmented with FOLLOW-set lookahead — reduce by $A \to \alpha$ only when the next token is in $\mathrm{FOLLOW}(A)$. Stronger than LR(0), weaker than LALR(1), cheap to construct.

## Key formulas

- Parse time: $O(n)$
- Reduce on $A \to \alpha$ allowed iff lookahead $\in \mathrm{FOLLOW}(A)$.
- Power: LR(0) $\subsetneq$ SLR(1) $\subsetneq$ LALR(1) $\subsetneq$ LR(1).

