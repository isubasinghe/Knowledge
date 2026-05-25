# Bloom filter

## Basic idea

A probabilistic set: tells you whether an element is *possibly in* the set or *definitely not*. Uses $k$ hash functions to set bits in an $m$-bit array. Cannot have false negatives; false-positive rate is tunable.

## Key formulas

- False-positive rate: $p \approx \left(1 - e^{-kn/m}\right)^k$
- Optimal $k$: $k^* = (m/n)\ln 2$
- Bits per element for FP rate $p$: $m/n = -\log_2 p / \ln 2 \approx 1.44 \log_2(1/p)$

