# Algebraic Data Type \(ADT\)

## Basic idea

Types built from sum (`|`, tagged union) and product (`,`, tuple/record) constructors. Pattern matching deconstructs them safely; exhaustiveness checks are decidable. The lingua franca of typed functional programming.

## Key formulas

- Cardinality: $|A + B| = |A| + |B|$; $|A \times B| = |A| \cdot |B|$
- Sum: `data T = L Int | R Bool` ⇒ $|T| = |\text{Int}| + |\text{Bool}|$
- Product: `data Pair = P Int Bool` ⇒ $|\text{Pair}| = |\text{Int}| \cdot |\text{Bool}|$
- Recursive: $\text{List}(A) \cong 1 + A \times \text{List}(A)$ ⇒ $L = 1/(1-A)$ formal solution.

