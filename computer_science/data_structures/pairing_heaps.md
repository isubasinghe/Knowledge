# Pairing heaps

## Basic idea

A heap-ordered multiway tree whose operations are defined by simple, lazy melding. Simpler and faster in practice than Fibonacci heaps, with surprisingly good (and still not fully analysed) amortised complexity.

## Key formulas

- find-min, insert, meld: $O(1)$
- decrease-key: $O(\log n)$ amortised (open: conjectured $o(\log n)$)
- delete-min: $O(\log n)$ amortised

