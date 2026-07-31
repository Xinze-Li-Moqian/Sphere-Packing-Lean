---
id: 44296aa079cf
type: lemma
from: blueprint
lean:
  - E8_norm_eq_sqrt_even
formalized: true
---

# Lemma — E8-vector-norms

## Statement

> [!lemma] E8-vector-norms
> All vectors in $\Lambda_8$ have norm of the form $\sqrt{2n}$, where $n$ is a nonnegative integer.

**In terms of**: [[e8-set]].

## Proof

> [!note]- Proof (click to expand)
> Writing $\vec{v} = \sum_i c_i\mathcal{B}_8^i$, we have $\|v\|^2 = \sum_i \sum_j c_ic_j (\mathcal{B}_8^i \cdot \mathcal{B}_8^j)$. Computing all $64$ pairs of dot products and simplifying, we get a massive term that is a quadratic form in $c_i$ with even integer coefficients, concluding the proof.

**Uses**: [[e8-defs-equivalent]].
