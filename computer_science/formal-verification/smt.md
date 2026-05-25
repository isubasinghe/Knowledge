# SMT based verification

## Basic idea

Encode program correctness obligations as formulas in a decidable first-order theory (arithmetic, arrays, bitvectors, uninterpreted functions, …) and discharge them with an SMT solver. The basis of modern auto-active verifiers (Dafny, Verus, Prusti, Boogie).

## Key formulas

- Hoare triple: $\{P\}\ C\ \{Q\}$
- Verification condition: $P \land \mathrm{wp}(C, Q) \models \bot$? (SMT-encoded)
- DPLL(T): SAT search modulo decision procedures for each theory $T$.

## Tools 
  * Verus (I worked on this at ETH Zuerich) 
  * Dafny 
  * Prusti

## Libraries 
  * https://hackage.haskell.org/package/sbv
