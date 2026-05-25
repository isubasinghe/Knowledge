# semantics

## Basic idea

Formal meaning of programs. Three classical styles: *operational* (how it runs, step-by-step), *denotational* (what mathematical object it denotes), *axiomatic* (which logical properties hold).

## Key formulas

- Small-step: $e \to e'$
- Big-step: $e \Downarrow v$
- Denotational: $\llbracket e \rrbracket : \text{Env} \to \text{Val}$
- Hoare triple (axiomatic): $\{P\}\ C\ \{Q\}$

