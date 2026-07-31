---
id: 07cbf27596d4
type: definition
from: blueprint
lean:
  - Θ₂
  - Θ₃
  - Θ₄
formalized: true
---

# Definition — def:th00-th01-th10

## Statement

> [!definition] def:th00-th01-th10
> We define three different theta functions (so called “Thetanullwerte”) as
> $$
> \begin{aligned}
> \Theta_{2}(z) = \theta_{10}(z)\,=\, & \sum_{n\in\mathbb{Z}}e^{\pi i (n+\frac12)^2 z}. \notag \\
> \Theta_{3}(z) = \theta_{00}(z)\,=\, & \sum_{n\in\mathbb{Z}}e^{\pi i n^2 z} \notag \\
> \Theta_{4}(z) = \theta_{01}(z)\,=\, & \sum_{n\in\mathbb{Z}}(-1)^n\,e^{\pi i n^2 z} \notag \\
> \end{aligned}
> $$

**Used by**: [[def-h2-h3-h4]], [[lemma-jacobi-identity]], [[lemma-theta-transform-s-t]].

## Notes

> [!note]- Notes (click to expand)
> - The name records that these are theta *values* — the classical $\theta(z,\tau)$ at $z = 0$ — so they are functions of the modular variable alone and belong to the same world as the [[def-ek|Eisenstein series]].
> - They satisfy the Jacobi identity $\theta_{00}^4 = \theta_{01}^4 + \theta_{10}^4$ ([[lemma-jacobi-identity]]), which is what makes the ring they generate small enough to compute in.
> - [[def-h2-h3-h4|$H_2, H_3, H_4$]] are built from them, and through those they enter the $-1$ eigenfunction; [[def-disc-definition|$\Delta$]] is their product up to a constant.
