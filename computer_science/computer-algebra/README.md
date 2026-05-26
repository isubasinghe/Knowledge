# computer\_algebra

## Basic idea

Exact, symbolic manipulation of mathematical expressions — polynomials, rational functions, ideals — as opposed to floating-point approximation. Core machinery includes Gröbner bases, resultants, and modular methods; powers systems like SageMath, Mathematica, and SymPy.

## Key facts

- Ideal membership, polynomial system solving, and elimination all reduce to Gröbner basis computation.
- Buchberger's algorithm (1965) is the original construction; F4/F5 (Faugère) are modern, much faster variants.
- Worst-case complexity is doubly exponential in the number of variables; in practice depends heavily on monomial order (lex vs grevlex).
