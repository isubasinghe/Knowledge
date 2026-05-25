# GeoHash

## Basic idea

Encodes (lat, lon) as a short base-32 string by interleaving the bits of each coordinate (Z-order). Common prefix length ≈ proximity, so adjacent points usually share long prefixes — handy for range queries on a B-tree or KV store.

## Key formulas

- Bits used for $n$-char geohash: $5n$
- Precision (cell side length) shrinks by factor 2 every extra bit; halves alternately in lat / lon.
- Distance bound: $d \le \sqrt{2} \cdot \text{cell diagonal}$ for same-prefix cells.

#### Resources

- https://en.wikipedia.org/wiki/Geohash
