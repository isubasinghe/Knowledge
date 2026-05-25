# Separation Logic

## Basic idea

An extension of Hoare logic for reasoning about heap-manipulating programs. Adds a separating conjunction $P * Q$ that asserts "$P$ and $Q$ hold of *disjoint* parts of the heap" — making local reasoning (the frame rule) sound.

## Key formulas

- Hoare triple: $\{P\}\ C\ \{Q\}$
- Separating conjunction: $P * Q$ — disjoint heap pieces
- Points-to: $x \mapsto v$ — heap cell at address $x$ holds $v$
- Frame rule: $\dfrac{\{P\}\ C\ \{Q\}}{\{P * R\}\ C\ \{Q * R\}}$ provided $C$ doesn't modify $\mathrm{fv}(R)$
- Magic wand: $P \mathbin{-\!*} Q$
