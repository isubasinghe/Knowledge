# search

## Basic idea

Locating items matching a query in a large corpus. Information-retrieval search uses an inverted index plus a ranking function (TF-IDF, BM25); algorithmic search explores combinatorial state spaces.

## Key formulas

- TF-IDF: $\text{tfidf}(t,d) = tf(t,d) \cdot \log\dfrac{N}{df(t)}$
- BM25: $\text{score}(d,q) = \sum_t \text{IDF}(t)\,\dfrac{tf(t,d)(k_1+1)}{tf(t,d) + k_1(1-b+b\,|d|/\overline{|d|})}$

