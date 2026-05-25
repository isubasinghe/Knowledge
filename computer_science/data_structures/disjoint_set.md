# Disjoint Set

## Basic idea

Union-find: tracks a partition of a set under merge (union) and lookup-root (find). With union-by-rank plus path compression, both operations run in inverse-Ackermann amortised time — essentially constant.

## Key formulas

- Amortised time per operation: $O(\alpha(n))$ with union-by-rank + path compression
- Sequence of $m$ ops on $n$ elements: $O(m\,\alpha(n))$ total
- Without optimisations: $O(\log n)$ per op

#### Resources

- https://en.wikipedia.org/wiki/Disjoint-set_data_structure
- https://dercuano.github.io/notes/incremental-union-find.html
