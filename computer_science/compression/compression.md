# Compression

## Basic idea

Map data to shorter codewords so that frequent symbols/sequences get short codes. Optimal codelengths are $-\log_2 P(x)$ (Shannon).

## Key formulas

- Shannon source-coding bound: $\bar L \ge H(X)$
- Kraft inequality (prefix codes): $\sum_i 2^{-l_i} \le 1$
- Huffman: greedy build of optimal prefix code; expected length $\bar L < H(X)+1$
- Arithmetic coding: encodes whole message as fractional interval; achieves $\bar L \to H(X)$

Huffman coding Arithmetic encoding

