# Adaptive Radix Tree

## Basic idea

A radix tree whose internal nodes adapt their fan-out (4/16/48/256) to actual key density at each level. Keeps the cache-friendliness of dense arrays for hot nodes while bounding memory for sparse ones. Comparable to hash tables but ordered.

## Key formulas

- Lookup/insert/delete: $O(k)$ where $k$ is key length in bytes (independent of $n$)
- Space: $O(n \cdot k)$ worst-case, much less in practice
- Node sizes: 4 / 16 / 48 / 256 entries

