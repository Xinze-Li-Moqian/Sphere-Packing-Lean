---
id: 67b2d3673adf
type: lemma
from: blueprint
lean:
  - EisensteinSeries.eisensteinSeries_SIF
---

# Lemma — lemma:Ek-is-modular-form

## Statement

> [!lemma] lemma:Ek-is-modular-form
> For all $k$, $E_k\in M_k(\Gamma_1)$.
> Especially, we have
> $$
> E_k \left(-\frac{1}{z}\right) = z^k E_k(z).
> $$

**In terms of**: [[def-mk]], [[def-gamma-1-action]], [[def-ek]].

## Proof

> [!note]- Proof (click to expand)
> This follows from the fact that the sum converges absolutely.
> Now apply [[def-slash-operator|slash operator]] with $\gamma = \left(\begin{smallmatrix} 0 & -1 \\ 1 & 0 \end{smallmatrix}\right)$ gives [[eq-ek-trans-s]].

**Uses**: [[def-ek]], [[def-mk]].
