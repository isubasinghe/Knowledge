# Dafny

## Basic idea

An auto-active verification language: programs are annotated with pre/post conditions, invariants, and termination measures; Dafny discharges the resulting proof obligations to the Z3 SMT solver.

## Key formulas

- Hoare triple: $\{P\}\ C\ \{Q\}$
- Loop invariant must hold: before loop, after each iteration, ⇒ post-condition on exit.
- Termination via lexicographic *decreases* clause.

## Resources 
  * https://dafny.org/dafny/OnlineTutorial/Lemmas.html
