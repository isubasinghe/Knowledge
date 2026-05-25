# Fibonacci heaps

## Basic idea

A heap of rooted trees with lazy consolidation. Achieves $O(1)$ amortised for insert and decrease-key, making Dijkstra and Prim run in $O(E + V\log V)$. Heavy hidden constants make it more theoretical than practical.

## Key formulas

- insert, find-min, merge, decrease-key: $O(1)$ amortised
- delete-min, delete: $O(\log n)$ amortised
- Max degree of any node: $D(n) \le \log_\phi n$

