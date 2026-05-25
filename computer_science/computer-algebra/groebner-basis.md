# Groebner basis

## Basic idea

A canonical generating set for a polynomial ideal under a chosen monomial order. Computing one (via Buchberger or F4/F5) is the "Gaussian elimination of polynomial systems": it lets you decide ideal membership, solve nonlinear systems, and simplify polynomial expressions.

## Key formulas

- $G = \{g_1, \dots, g_s\}$ is a Gröbner basis of ideal $I$ iff $\langle LT(I) \rangle = \langle LT(g_1), \dots, LT(g_s) \rangle$
- S-polynomial: $S(f,g) = \dfrac{\mathrm{lcm}(LM(f),LM(g))}{LT(f)} f - \dfrac{\mathrm{lcm}(LM(f),LM(g))}{LT(g)} g$
- Buchberger's criterion: $G$ is Gröbner iff every $S(g_i,g_j)$ reduces to $0$ modulo $G$.

## Resources 
  * https://en.wikipedia.org/wiki/Computer_algebra
