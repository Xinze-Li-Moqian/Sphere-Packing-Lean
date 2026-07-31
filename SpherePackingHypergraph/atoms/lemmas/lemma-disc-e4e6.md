---
id: e5e2d5eabf21
type: lemma
from: blueprint
lean:
  - ModularForm.discriminant_eq_E₄_cube_sub_E₆_sq
formalized: true
---

# Lemma — lemma:disc-E4E6

## Statement

> [!lemma] lemma:disc-E4E6
> We have
> $$
> \Delta(z) = (E_4^3-E_6^2)/1728.
> $$

## Proof

> [!note]- Proof (click to expand)
> We only need to show its a cuspform, since once we have this, dividing the rhs by $\Delta$ would give a [[def-mk|modular form]] of weight $0$ which is a constant, and so we can determine the constant easily.
> 
> To check its a cuspform, we just look at  the $q$-expansions of $E_4$ and $E_6$ and prove directly that the first term vanishes.
