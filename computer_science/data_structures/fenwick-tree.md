# Fenwick tree

## Basic idea

Binary-indexed tree: an array that supports prefix-sum queries and point updates in $O(\log n)$ using bit tricks on the index. Smaller and faster constants than a segment tree when only prefix sums are needed.

## Key formulas

- Update index $i$: $i \mathrel{+}= i \mathbin{\&} -i$
- Query prefix sum up to $i$: $i \mathrel{-}= i \mathbin{\&} -i$
- Range sum $[l,r]$: $\text{prefix}(r) - \text{prefix}(l-1)$
- Time: $O(\log n)$ per op; Space: $O(n)$

## Resources 
  * https://en.wikipedia.org/wiki/Fenwick_tree
