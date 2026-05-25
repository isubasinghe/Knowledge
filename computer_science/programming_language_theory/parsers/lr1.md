# LR\(1\) parser

## Basic idea

Canonical LR(1): each state remembers an exact 1-token lookahead, so it accepts every deterministic CFG. Tables are large; LALR(1) is the practical compromise that merges equivalent LR(1) states.

## Key formulas

- Parse time: $O(n)$
- LR(1) item: $[A \to \alpha \cdot \beta, a]$ where $a$ is the lookahead.
- Strictly more powerful than SLR(1) / LALR(1); accepts all deterministic CFLs.

