# Equality Saturation

## Basic idea

Represent a program as an *e-graph* — a data structure encoding many equivalent expressions at once — then apply rewrite rules until no new equalities are discovered. Pick the cheapest member of the resulting equivalence class. Avoids the phase-ordering problem of traditional optimisers.

## Key facts

- E-graph: union-find of *e-classes*; each e-class holds e-nodes; equality propagates via *upward merging*.
- Phase: build → saturate (apply rules) → extract minimum-cost program.
- Implementation: egg (Rust); used by Cranelift, Herbie, Glenside, Tensat, etc.

## Resources
  * https://docs.rs/egg/latest/egg/
