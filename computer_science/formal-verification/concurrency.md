# Handling Concurrency in Formal Verification.

## Basic idea

Proving concurrent programs correct requires reasoning about interleavings or about shared state under interference. Modern approaches use concurrent separation logic (CSL) and Iris-style frameworks to make these proofs scale.

## Key formulas

- Owicki-Gries: interference freedom of every assertion against every other thread's step.
- Rely/Guarantee: $\{P, R\}\ C\ \{G, Q\}$ — $R$ is what env may do, $G$ is what $C$ promises.
- CSL frame rule: $\dfrac{\{P\}\ C\ \{Q\}}{\{P*R\}\ C\ \{Q*R\}}$ when $C$ doesn't touch $R$'s heap.

## Concurrency is in my opinion a solved problem.

Not to cite my own work but Verus shows how IronSync style proofs can scale.


## Resources
  * https://dl.acm.org/doi/pdf/10.1145/3586037
