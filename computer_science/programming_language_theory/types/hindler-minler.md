# Hindler-Milner type system

## Basic idea

A polymorphic type system that admits *principal* types and full type *inference* without annotations (Algorithm W). Foundation of ML, Haskell, OCaml.

## Key formulas

- Typing rule (Var): $\dfrac{x : \sigma \in \Gamma}{\Gamma \vdash x : \mathrm{inst}(\sigma)}$
- Typing rule (Abs): $\dfrac{\Gamma, x:\tau_1 \vdash e : \tau_2}{\Gamma \vdash \lambda x.e : \tau_1 \to \tau_2}$
- Generalisation: $\mathrm{gen}(\Gamma, \tau) = \forall \bar\alpha.\ \tau$ where $\bar\alpha = \mathrm{ftv}(\tau) \setminus \mathrm{ftv}(\Gamma)$
- Algorithm W: type inference via unification; produces *principal* type.
- Let-polymorphism only — no first-class polymorphism (system F is needed for that).

