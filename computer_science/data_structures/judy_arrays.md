# Judy Arrays

## Basic idea

A cache-conscious associative array invented at HP Labs. Internally a 256-way digital trie that switches between several node layouts to minimise both cache misses and memory. Very fast — but the implementation is notoriously complex.

## Key formulas

- Lookup/insert/delete: $O(\log_{256} n)$ — effectively constant.
- Memory: $\approx 8$ bytes per element typical, much less than a hash table at small sizes.

Are an associative data structure which tends to have better performance than heaps. It comes with other benefits as well, since it an array, it is more cache friendly.

## Why is this not more common?

The performance improvement is not worth the complexity of the implementation

## Interesting facts

Douglas Baskins named this after his sister, Judy.

