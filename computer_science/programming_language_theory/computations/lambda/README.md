# lambda

## Basic idea

The $\lambda$-calculus: a minimal formal system of variables, abstraction $\lambda x.\, e$, and application $e_1\, e_2$. Turing-complete in three rules; the theoretical core of every functional language.

## Key formulas

- Syntax: $e ::= x \mid \lambda x.\, e \mid e\, e$
- $\beta$-reduction: $(\lambda x.\, e)\, v \to e[v/x]$
- $\eta$-conversion: $\lambda x.\, f\, x \equiv f$ (when $x \notin \mathrm{fv}(f)$)
- Church-Rosser: reduction is confluent — normal forms are unique up to $\alpha$-equivalence.
