# AIXI

## Basic idea

A theoretical mathematical formalism for artificial general intelligence (Marcus Hutter, 2000). Combines Solomonoff induction (universal prior over environments) with sequential decision theory: the agent picks the action that maximises expected future reward summed over all computable environments, weighted by Kolmogorov complexity.

## Key formulas

- $a_k = \arg\max_{a_k} \sum_{o_k r_k} \cdots \max_{a_m} \sum_{o_m r_m} (r_k + \cdots + r_m) \sum_{q : U(q,a_{1..m}) = o_1 r_1 \cdots o_m r_m} 2^{-|q|}$
- Universal prior: $\xi(x) = \sum_{p : U(p)=x*} 2^{-|p|}$
- Uncomputable, but $\varepsilon$-approximable.

Is a theoritical mathematical formalism for artificial general intelligence. AIXI was first proposed by Marcus Hutter.

## Resources

[https://en.wikipedia.org/wiki/AIXI](https://en.wikipedia.org/wiki/AIXI)

