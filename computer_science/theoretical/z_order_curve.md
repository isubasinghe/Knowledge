# Z-order curve

## Basic idea

A space-filling curve (Morton order) that maps multidimensional coordinates to one dimension by *interleaving* the bits of the coordinates. Cheaper to compute than Hilbert; preserves locality moderately well.

## Key formulas

- 2D Morton encoding: $z(x,y) = \sum_{i} (x_i \cdot 4^i \cdot 2 + y_i \cdot 4^i)$ — interleave bits.
- $z(x,y,z) = $ interleave 3 streams of bits.
- Resulting order = depth-first traversal of a quadtree (2D) / octree (3D).

In mathematical analysis and computer science, functions which are Z-order, Lebesgue curve, Morton space filling curve, Morton order or Morton code map multidimensional data to one dimension while preserving locality of the data points. It is named after Guy Macdonald Morton, who first applied the order to file sequencing in 1966. The z-value of a point in multidimensions is simply calculated by interleaving the binary representations of its coordinate values. Once the data are sorted into this ordering, any one-dimensional data structure can be used such as binary search trees, B-trees, skip lists or \(with low significant bits truncated\) hash tables. The resulting ordering can equivalently be described as the order one would get from a depth-first traversal of a quadtree.

## Resources

* [https://en.wikipedia.org/wiki/Z-order\_curve](https://en.wikipedia.org/wiki/Z-order_curve)

