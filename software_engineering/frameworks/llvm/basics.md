# LLVM Basics

## Basic idea

A toolkit of reusable compiler passes over a typed SSA IR. Front-ends emit LLVM IR; opt runs analysis/transform passes; llc lowers it to a target ISA. Decouples language design from back-end engineering.

## Key facts

- IR is SSA-form, statically typed, three-address.
- Pass kinds: analysis (read-only) and transform.
- Key tools: `clang`, `opt`, `llc`, `lld`, `lli`.
- Phi nodes select values at CFG join points.

