# Hash Tables

## Basic idea

Map keys to slots via a hash function. With a good hash, lookups average $O(1)$. Collision handling (chaining, open addressing) and load factor determine performance.

## Key formulas

- Load factor: $\lambda = n/m$
- Expected chain length (chaining): $\lambda$
- Open addressing probe count (uniform hashing): $\approx \dfrac{1}{1-\lambda}$ (successful), $\dfrac{1}{(1-\lambda)^2}$ (unsuccessful)

### Poisson distribution
Consider a hash table with **m** slots and **n** elements in it. 
Denote the load factor by λ=(n/m). The probability that a given 
slot has **k** elements is given by 

<img align="center" src="https://i.upmath.me/svg/P(k%3B%20%5Clambda)%20%3D%20%5Cfrac%7Be%5E%7B-%5Clambda%7D%20%5Clambda%5Ek%7D%7Bk!%7D" alt="P(k; \lambda) = \frac{e^{-\lambda} \lambda^k}{k!}" />

