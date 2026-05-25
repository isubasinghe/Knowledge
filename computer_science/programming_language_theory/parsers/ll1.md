# LL1 parser

## Basic idea

Top-down, predictive parser using a single token of lookahead. Either hand-coded as recursive-descent functions, or table-driven from a FIRST/FOLLOW analysis. Fast and gives great error messages — at the price of grammar restrictions (no left recursion, no common prefixes).

## Key formulas

- Parse time: $O(n)$, space $O(\text{depth})$ for recursive descent.
- Predict set: $\mathrm{PREDICT}(A \to \alpha) = \mathrm{FIRST}(\alpha) \cup (\mathrm{FOLLOW}(A)$ if $\varepsilon \in \mathrm{FIRST}(\alpha))$.
- LL(1) condition: predict sets of alternatives for the same nonterminal are pairwise disjoint.

Two types: hand coded recursive descent which is essentially LL\(\*\) or table driven.

