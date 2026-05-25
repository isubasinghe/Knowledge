# compression

## Basic idea

Encoding data with fewer bits by exploiting statistical structure. Lossless compression is bounded below by Shannon entropy; lossy compression trades fidelity for size.

## Key formulas

- Shannon source-coding bound: $\bar L \ge H(X)$
- Kraft inequality: $\sum_i 2^{-l_i} \le 1$
- Shannon entropy: $H(X) = -\sum_i p_i \log_2 p_i$

