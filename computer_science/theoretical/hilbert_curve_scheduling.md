# Hilbert curve scheduling

## Basic idea

A load-balancing technique that orders multidimensional tasks along a Hilbert curve and partitions that 1D sequence among workers — preserving spatial locality of work, so neighbouring tasks tend to land on the same worker.

## Key facts

- Reduces communication between neighbouring partitions vs. row-major partitioning.
- Used in N-body simulations, AMR, parallel mesh codes.
- Tradeoff: better locality at the cost of more complex indexing.

## Resources

* [https://en.wikipedia.org/wiki/Hilbert\_curve\_scheduling](https://en.wikipedia.org/wiki/Hilbert_curve_scheduling)

