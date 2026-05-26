# formal\_verification

## Basic idea

Mathematically proving that a program (or hardware design) satisfies a specification, rather than testing it on sample inputs. Approaches range from automated SMT-based checking (Z3, Dafny) to interactive proof assistants and dedicated logics for state, heap, and concurrency.

## Key facts

- **SMT** (Satisfiability Modulo Theories): SAT extended with theories of integers, reals, arrays, bitvectors — Z3, CVC5.
- **Separation logic**: extension of Hoare logic with $P * Q$ for disjoint heaps; enables the frame rule and local reasoning.
- **Weak memory models**: x86-TSO, ARMv8, C11 — reasoning about reorderings under relaxed consistency.
- **Dafny / Viper**: program verifiers that discharge proof obligations to SMT solvers.
