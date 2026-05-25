# CTrie

## Basic idea

A concurrent, lock-free hash array mapped trie (HAMT) with O(1) snapshots via persistent, copy-on-write generation counters. Supports linearisable read/update plus consistent atomic iteration.

## Key formulas

- Lookup/insert/delete: $O(\log_{32} n)$ expected (32-way branching)
- Snapshot: $O(1)$ amortised
- Memory: $O(n)$

## Resources 
  * http://aleksandar-prokopec.com/resources/docs/ctries-snapshot.pdf
