# Attribute grammars

## Basic idea

Augment a CFG by attaching *attributes* to grammar symbols and *semantic rules* that compute them. A clean way to fold static analysis (type checking, scope resolution) directly into parsing.

## Key facts

- *Synthesised* attributes flow up from children to parent.
- *Inherited* attributes flow down from parent / siblings.
- S-attributed: only synthesised — evaluable in one bottom-up pass (yacc-friendly).
- L-attributed: synthesised + inherited-from-left-siblings — evaluable in one left-to-right pass (LL-friendly).

1. S-attributed grammars
2. L-attributed grammars

