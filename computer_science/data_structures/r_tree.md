# R tree

## Basic idea

A height-balanced tree of minimum bounding rectangles (MBRs). Each internal node groups its children's MBRs into a parent MBR, so a spatial query descends only into subtrees whose MBR overlaps the query.

## Key formulas

- Query / insert / delete: $O(\log_M n)$ where $M$ is node fan-out
- Pruning condition: skip subtree if $\text{MBR} \cap \text{query} = \emptyset$
- Variants: R*-tree (better splits), R+-tree, Hilbert R-tree.

#### Resources

- https://en.wikipedia.org/wiki/R-tree
