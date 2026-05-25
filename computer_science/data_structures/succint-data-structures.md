# Succint Datastructures

## Basic idea

Data structures whose space usage is information-theoretically optimal *plus a lower-order term*, while still supporting fast queries. Example: a bit-vector with rank/select in $O(1)$ using $n + o(n)$ bits.

## Key formulas

- Succinct: space $= Z + o(Z)$ where $Z$ is the information-theoretic lower bound
- Compact: $O(Z)$ bits
- rank/select on bit-vectors: $O(1)$ time, $o(n)$ extra bits

## Resources
  * http://stevehanov.ca/blog/?id=120
