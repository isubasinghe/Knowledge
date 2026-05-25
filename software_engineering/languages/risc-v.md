# RISC-V

## Basic idea

An open, royalty-free, modular RISC ISA from UC Berkeley (2010). 32 GP registers, fixed 32-bit instructions in the base, optional extensions (M, A, F, D, C, V, …). Designed for clean teaching and clean implementation.

## Key facts

- Year / origin: 2010, UC Berkeley.
- Base: RV32I / RV64I / RV128I — load/store, fixed 32-bit ops (16-bit with `C` extension).
- 32 GP registers (`x0`-`x31`); `x0` hardwired to 0.
- Calling convention: args in `a0`-`a7`, return in `a0`/`a1`, link in `ra`.
- Extensions: M (mult/div), A (atomics), F/D (float), C (compressed), V (vector).

## Resources 
  * https://maskray.me/blog/2022-07-10-riscv-linker-relaxation-in-lld
