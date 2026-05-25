# Weak Memory Models

## Basic idea

Real CPUs (x86-TSO, ARM, RISC-V, POWER) reorder loads and stores aggressively for performance, so the program order you write is *not* the order other cores observe. Verifying concurrent code requires modelling these reorderings precisely.

## Key facts

- x86-TSO: only store→load reorderings allowed (FIFO store buffer per core).
- ARM/Power: nearly any reordering allowed; require explicit barriers (`dmb`, `lwsync`).
- C++11 memory_order: relaxed / acquire / release / acq_rel / seq_cst.
- Operational and axiomatic (cat-language) models coexist.

Work on verifying weak memory models represents the frontier of verification research in my opinion (as of 2025 at least).
