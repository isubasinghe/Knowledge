# Affine types

## Basic idea

Substructural type system in which a value of an affine type may be used *at most once*. Weaker than linear (which requires *exactly once*); the backbone of Rust's ownership model.

## Key formulas

- Contraction is disallowed: $\Gamma, x:\tau, x:\tau \not\vdash$
- Weakening is allowed: $\Gamma \vdash e : \sigma \implies \Gamma, x:\tau \vdash e : \sigma$
- Rust: each owned value is dropped (deallocated) at end of scope if not moved.

