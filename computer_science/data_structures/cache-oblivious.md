# Cache Oblivious Algorithms & Datastructures

## Basic idea

Algorithms that achieve optimal cache performance *without knowing* the cache parameters (line size, capacity). They work well across every level of the memory hierarchy simultaneously, typically via recursive divide-and-conquer.

## Key formulas

- External-memory model: cost = number of $B$-sized block transfers between cache and memory.
- Optimal cache-oblivious sort: $O\!\left(\dfrac{n}{B}\log_{M/B}\dfrac{n}{B}\right)$ transfers.
- van Emde Boas layout for trees: $O(\log_B n)$ block accesses per search.

## Resources 
  * https://cs.au.dk/~gerth/MassiveData02/notes/demaine.pdf
