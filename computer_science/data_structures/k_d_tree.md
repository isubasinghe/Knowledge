# k-d Tree

## Basic idea

A BST over $k$-dimensional points that cycles the splitting axis at each level. Good for nearest-neighbour and range queries in low dimensions; degrades badly as $k$ grows ("curse of dimensionality").

## Key formulas

- Build: $O(n \log n)$
- Range / nearest-neighbour search: $O(\sqrt n)$ in 2D balanced, $O(n^{1-1/k} + r)$ general worst case
- Effective only while $k \lesssim 20$.

#### Resources

- https://en.wikipedia.org/wiki/K-d_tree
