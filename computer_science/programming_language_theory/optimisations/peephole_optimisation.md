# Peephole optimisation

## Basic idea

Slide a small window over the instruction stream and replace short patterns with cheaper equivalents (e.g. `mul x, 2` → `shl x, 1`; `mov a, b; mov b, a` → `mov a, b`). Cheap, local, and surprisingly effective at the end of the pipeline.

## Key facts

- Window typically 2-5 instructions.
- Rules are target-specific (instruction selection's afterburn).
- Modern compilers often implement these as e-graph rewrites or table-driven patterns.

