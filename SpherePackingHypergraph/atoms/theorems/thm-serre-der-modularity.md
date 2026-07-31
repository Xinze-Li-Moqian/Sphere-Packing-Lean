---
id: b0d10d303b0b
type: theorem
from: blueprint
lean:
  - serre_D_slash_invariant
formalized: true
---

# Theorem — thm:serre-der-modularity

## Statement

> [!theorem] thm:serre-der-modularity
> Let $F$ be a [[def-mk|modular form]] of weight $k$ and level $\Gamma$. Then, $\partial_{k}F$ is a modular form of weight $k + 2$ of the same level.

## Proof

> [!note]- Proof (click to expand)
> Immediate from Theorem [[thm-serre-der-equiv-action]] since $F|_k\gamma = F$ for all $\gamma \in \Gamma$.
