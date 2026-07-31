---
id: 425210f2bd51
type: definition
from: blueprint
lean:
  - UpperHalfPlane.denom
formalized: true
---

# Definition — def:automorphy-factor

## Statement

> [!definition] def:automorphy-factor
> The *automorphy factor* of weight $k$ is defined as
> $$j_k(z,\left(\begin{smallmatrix}a&b\\c&d\end{smallmatrix}\right)):=(cz+d)^{-k}.$$

**Used by**: [[def-slash-operator]], [[lemma-automorphy-factor-chain-rule]].

## Notes

> [!note]- Notes (click to expand)
> - $c$ and $d$ are the bottom row of the matrix [[def-gamma-1-action|acting]] on $z$; the factor is exactly the derivative of that action, up to a power.
> - It is a cocycle: $j_k(z, \gamma_1\gamma_2) = j_k(\gamma_2 z, \gamma_1)\, j_k(z, \gamma_2)$, which is why the [[def-slash-operator|slash operator]] built from it is a group action and why [[lemma-slash-operator-chain-rule]] holds.
> - A [[def-mk|modular form]] of weight $k$ is a function invariant under the slash operator — that is, one that transforms by this factor and nothing else.
