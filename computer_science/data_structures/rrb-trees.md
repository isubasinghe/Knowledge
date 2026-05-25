# RRB-Trees

## Basic idea

Relaxed Radix Balanced trees: a persistent vector that adds $O(\log n)$ concat and split to Clojure-style 32-way trie vectors by allowing slightly-unbalanced subtrees ("relaxed" nodes carry a size table).

## Key formulas

- Lookup / update / append: $O(\log_{32} n)$ — effectively constant
- Concat / split: $O(\log n)$
- Branching factor: 32

##Resources 
  * [EPFL](https://os.zhdk.cloud.switch.ch/tind-tmp-epfl/b835df0d-9cc6-44a1-a7f6-37e0ffcdf8cc?response-content-disposition=attachment%3B%20filename%2A%3DUTF-8%27%27RMTrees.pdf&response-content-type=application%2Fpdf&AWSAccessKeyId=ded3589a13b4450889b2f728d54861a6&Expires=1658739560&Signature=wVIlhsoQttwVv9zwPXvdCw3DLUs%3D)
