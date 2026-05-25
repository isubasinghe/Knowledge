# M Tree

## Basic idea

A balanced tree for similarity search in *generic metric spaces* (any distance satisfying the triangle inequality), not just Euclidean. Stores routing objects with covering radii so the triangle inequality can prune subtrees during search.

## Key formulas

- Triangle inequality: $d(x,z) \le d(x,y) + d(y,z)$
- Pruning rule: skip subtree at routing object $r$ with radius $\rho$ if $d(q, r) > \varepsilon + \rho$ for $\varepsilon$-range query.
- Range / kNN query: $O(\log n)$ in low intrinsic dimension.

#### Resources

- https://en.wikipedia.org/wiki/M-tree
