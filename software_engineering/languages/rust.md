# Rust

## Basic idea

Systems language (Mozilla, 2010) that achieves memory safety without garbage collection via an ownership + borrowing type system enforced at compile time. Affine types in production.

## Key facts

- Year / creator: 2010 first release, Graydon Hoare at Mozilla.
- Paradigm: imperative + functional + trait-based generics.
- Typing: static, strong; type inference.
- Memory: ownership / borrowing (affine types); no GC.
- Concurrency: `Send` / `Sync` traits enforce data-race freedom at compile time.

