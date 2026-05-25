# Earley parser

## Basic idea

Bottom-up chart parser that handles *any* context-free grammar — including ambiguous and left-recursive ones. Maintains a set of "items" (dotted productions with a start index) per input position.

## Key formulas

- General CFG: $O(n^3)$
- Unambiguous CFG: $O(n^2)$
- Deterministic / LR-style grammar: $O(n)$
- Memory: $O(n^2)$

Can parse all CFG's but are slow

