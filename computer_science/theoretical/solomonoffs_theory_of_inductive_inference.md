# Solomonoff's theory of inductive inference

## Basic idea

A formal Bayesian theory of prediction: weight every computable hypothesis by $2^{-K(h)}$ (Occam's razor made precise). The resulting universal prior provably converges to the true distribution for any computable source.

## Key formulas

- Universal prior: $M(x) = \sum_{p : U(p) = x*} 2^{-|p|}$
- Conditional predictor: $M(x_{n+1} \mid x_{1..n}) = M(x_{1..n+1}) / M(x_{1..n})$
- Convergence: total expected squared error $\sum_n \mathbb{E}[(M(x_n|x_{<n}) - \mu(x_n|x_{<n}))^2] \le \tfrac{1}{2}\ln 2 \cdot K(\mu)$
- Uncomputable but lower-semicomputable.

## Resources

[https://en.wikipedia.org/wiki/Solomonoff%27s\_theory\_of\_inductive\_inference](https://en.wikipedia.org/wiki/Solomonoff%27s_theory_of_inductive_inference)

