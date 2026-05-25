# Hilbert-R Tree

## Basic idea

An R-tree whose leaf entries are ordered by the Hilbert value of their centroid. This deterministic, locality-preserving order gives much better split decisions and higher space utilisation than ordinary R-trees.

## Key formulas

- Hilbert value: $h = H(x,y)$ along an order-$n$ Hilbert curve
- Query / insert: $O(\log n)$
- Typical utilisation: ~95% (vs ~70% for R*-tree).

#### Resources

- https://en.wikipedia.org/wiki/Hilbert_R-tree
