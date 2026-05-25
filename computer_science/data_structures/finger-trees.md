# Finger-Trees

## Basic idea

A persistent functional sequence with cheap access at both ends and $O(\log n)$ split/concat. Generalises to many abstract structures (deques, priority queues, interval maps) via a *monoidal annotation*.

## Key formulas

- push/pop (either end): $O(1)$ amortised
- Concat: $O(\log\min(m, n))$
- Split / index: $O(\log n)$

## Resources
  * https://andrew.gibiansky.com/blog/haskell/finger-trees/
  * https://www.youtube.com/watch?v=ip92VMpf_-A
