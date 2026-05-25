# HyperLogLog 

## Basic idea

A streaming cardinality estimator that uses $O(\log\log n)$ bits per register. Hash each element, take the position of the first 1-bit in the low bits as a proxy for $\log_2$ of the (sub-stream) cardinality, then average across $m$ registers with the harmonic mean.

## Key formulas

- Estimate: $\hat n = \alpha_m \cdot m^2 \cdot \left(\sum_{j=1}^{m} 2^{-M_j}\right)^{-1}$
- Standard error: $\sigma \approx 1.04/\sqrt{m}$
- Constant: $\alpha_{16}=0.673,\ \alpha_{32}=0.697,\ \alpha_{64}=0.709,\ \alpha_m \to 1/(2\ln 2)$

## Resources 
  * https://en.wikipedia.org/wiki/HyperLogLog
