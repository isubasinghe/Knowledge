# llvm

## Basic idea

Modular compiler infrastructure (formerly "Low Level Virtual Machine") used as a back-end by Clang, Rust, Swift, Julia, and many others. The defining abstraction is a typed, SSA-based intermediate representation.

## Key facts

- IR: typed, SSA form, three-address.
- Pass pipeline: front-end → IR → passes (analysis + transform) → back-end → target machine code.
- Clang, MLIR, Cranelift, llgo all build on LLVM.

