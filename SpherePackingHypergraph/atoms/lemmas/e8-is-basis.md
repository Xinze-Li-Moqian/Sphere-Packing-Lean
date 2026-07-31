---
id: e2e5920410cc
type: lemma
from: blueprint
lean:
  - span_E8Matrix_eq_top
formalized: true
---

# Lemma — E8-is-basis

## Statement

> [!lemma] E8-is-basis
> $B_8$ is a $\mathbb{R}$-basis of $\mathbb{R}^8$.

**In terms of**: [[e8-matrix]].

## Proof

> [!note]- Proof (click to expand)
> It suffices to prove that $\mathcal{B}_8 \in \mathrm{GL}_8(\mathbb{R})$. We prove this by explicitly defining the inverse matrix $\mathcal{B}_8^{-1}$ and proving $\mathcal{B}_8 \mathcal{B}_8^{-1} = I_8$, which implies that $\det(\mathcal{B}_8)$ is nonzero. See the Lean code for more details.,

**Uses**: [[e8-matrix]].
