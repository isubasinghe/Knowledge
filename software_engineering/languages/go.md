# Go

## Basic idea

Statically typed, garbage-collected systems-ish language from Google (2009). Designed for simplicity, fast compilation, and CSP-style concurrency (goroutines + channels). Deliberately small feature set.

## Key facts

- Year / creator: 2009, Pike, Thompson, Griesemer at Google.
- Paradigm: imperative + structural typing + CSP concurrency.
- Typing: static, strong; type inference via `:=`.
- Memory: garbage-collected; escape analysis decides heap vs stack.
- Concurrency: goroutines (M:N scheduled), channels, `select`.

