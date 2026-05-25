# Kolmogorov complexity

## Basic idea

The Kolmogorov complexity $K(x)$ of a string $x$ is the length of the shortest program (for a fixed universal Turing machine) that outputs $x$. It is the formal notion of "intrinsic information content" — and it is uncomputable.

## Key formulas

- $K(x) = \min\{|p| : U(p) = x\}$
- Invariance theorem: $|K_U(x) - K_{U'}(x)| \le c_{U,U'}$ (machine-independent up to a constant)
- Most strings are incompressible: $|\{x \in \{0,1\}^n : K(x) < n-c\}| < 2^{n-c}$
- $K(x)$ is uncomputable (else we could solve the halting problem).

## Resources

[https://en.wikipedia.org/wiki/Kolmogorov\_complexity](https://en.wikipedia.org/wiki/Kolmogorov_complexity)

