# Segment Trees

## Basic idea

A balanced binary tree over array intervals: each node stores an aggregate (sum/min/gcd/…) of its range. Supports point/range update and range query in $O(\log n)$, and is far more flexible than a Fenwick tree (any associative op, lazy propagation).

## Key formulas

- Build: $O(n)$
- Range query / point update: $O(\log n)$
- Range update with lazy propagation: $O(\log n)$
- Space: $4n$ nodes

