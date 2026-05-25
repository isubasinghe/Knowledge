# Count-min sketch

## Basic idea

Probabilistic frequency estimator. A $d \times w$ array of counters, each row indexed by a different hash function: increment all $d$ cells on update, return the minimum on query. Always overestimates; never undercounts.

## Key formulas

- Estimate: $\hat f_x = \min_{i=1..d} CM[i, h_i(x)]$
- Width: $w = \lceil e/\varepsilon \rceil$
- Depth: $d = \lceil \ln(1/\delta) \rceil$
- Guarantee: $\hat f_x \le f_x + \varepsilon \|f\|_1$ with probability $\ge 1-\delta$

## Resources 
  * https://en.wikipedia.org/wiki/Count%E2%80%93min_sketch
