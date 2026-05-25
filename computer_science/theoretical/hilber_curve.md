# Hilbert Curve

## Basic idea

A continuous space-filling curve that maps $[0,1]$ onto $[0,1]^d$ while preserving locality: points close on the curve are close in space. Useful for spatial indexing and cache-friendly traversals.

## Key formulas

- Recursively defined; at iteration $n$ the curve visits $4^n$ cells (in 2D) of side $2^{-n}$.
- Distance on curve ↔ spatial distance bound: $\|p - q\|_2 \le c \cdot d_H(p,q)^{1/d}$
- Length of $n$-th order approximation: $L_n = 2^n - 2^{-n}$ (unit square).

## Resources

* [https://en.wikipedia.org/wiki/Hilbert\_curve](https://en.wikipedia.org/wiki/Hilbert_curve)

