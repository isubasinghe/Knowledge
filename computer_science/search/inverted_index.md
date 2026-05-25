# Inverted Index

## Basic idea

A map from term → posting list (the documents containing the term, often with positions). Lets a search engine answer "which docs contain word X?" in time proportional to the result size, not the corpus size.

## Key formulas

- Index size: $\sum_t |postings(t)|$
- Query (AND): intersect posting lists in $O(\sum |L_i|)$
- TF-IDF weight: $w(t,d) = tf(t,d) \cdot \log(N/df(t))$

For efficient storage of inverted indicies refer to ARTs \(Adaptive Radix Tree\)

