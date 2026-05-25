# Hash Array Mapped Tries

## Basic idea

A persistent associative map: a trie keyed by chunks of a hash, where each interior node stores only the populated children plus a bitmap saying which slots are filled. The basis of immutable maps in Clojure, Scala, Haskell.

## Key formulas

- Lookup/insert/delete: $O(\log_{32} n)$ (constant in practice — $\le 7$ steps for $n < 2^{32}$)
- Branching factor: $32$ (5 bits of hash per level)
- Path copying makes update $O(\log n)$ in space too.

## Resources 
  * https://worace.works/2016/05/24/hash-array-mapped-tries/
