# Sparse Sets

## Basic idea

A set of integers from $[0, U)$ stored as two arrays: `dense` (the elements) and `sparse` (positions of each element in `dense`). $O(1)$ insert / delete / membership / clear, with cache-friendly iteration over members.

## Key formulas

- All ops: $O(1)$ worst case (no hashing)
- Memory: $O(U + n)$ — high cost when $U \gg n$
- Cleared in $O(1)$ by zeroing the count.

## Resources 
  * https://research.swtch.com/sparse

