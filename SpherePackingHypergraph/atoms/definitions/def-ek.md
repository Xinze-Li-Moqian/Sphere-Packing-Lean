---
id: b5d7a849dfa1
type: definition
from: blueprint
lean:
  - ModularForm.eisensteinSeries_MF
---

# Definition — def:Ek

## Statement

> [!definition] def:Ek
> For an even integer $k\geq 4$ we define the *weight $k$ Eisenstein series* as
> $$
> E_k(z):=\frac{1}{2}\sum_{(c,d)\in\mathbb{Z}^2, (c,d)=1}(cz+d)^{-k}.$$

**Used by**: [[def-fg-definition]], [[def-phi4-phi2-phi0]], [[eq-ddf]], [[eq-ddg]].

## Notes

> [!note]- Notes (click to expand)
> - Each summand is an [[def-automorphy-factor|automorphy factor]] $(cz+d)^{-k}$, and summing over all coprime pairs is what forces the result to transform correctly: the sum is invariant because [[def-gamma-1-action|the group]] permutes the pairs.
> - The restriction to even $k \ge 4$ is not cosmetic. Odd $k$ gives zero by the $(c,d) \mapsto (-c,-d)$ symmetry, and $k = 2$ makes the sum conditionally convergent — the value one gets by summing anyway is $E_2$ ([[def-e2]]), which is not a modular form.
> - $E_k \in M_k(\Gamma_1)$ ([[def-mk]]), and $E_4, E_6$ generate the whole ring; $\Delta$ ([[def-disc-definition]]) is the first thing they build that vanishes at the cusp.
