# LR\(0\) parser

## Basic idea

Bottom-up shift-reduce parser with *zero* lookahead. Uses the canonical collection of LR(0) items as states; reduce whenever a final item is present. Weak — many grammars have shift/reduce or reduce/reduce conflicts here.

## Key formulas

- Parse time: $O(n)$
- States = items closed under $\mathrm{GOTO}$
- LR(0) item: $A \to \alpha \cdot \beta$
- Strictly weaker than SLR(1), LALR(1), LR(1).

