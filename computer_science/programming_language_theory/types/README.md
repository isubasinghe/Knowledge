# types

## Basic idea

Static disciplines that classify program values and rule out classes of errors before execution. Type systems range from simple (Hindley-Milner) to dependent (Coq, Lean) — more expressive types catch more errors but cost more to check.

## Key formulas

- Typing judgement: $\Gamma \vdash e : \tau$
- Function type: $\tau_1 \to \tau_2$
- Universal type: $\forall \alpha.\ \tau$
- Curry-Howard: types ≅ propositions; programs ≅ proofs.

