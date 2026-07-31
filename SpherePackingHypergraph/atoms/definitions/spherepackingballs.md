---
id: 8ac9d214b5a9
type: definition
from: blueprint
lean:
  - SpherePacking.balls
formalized: true
---

# Definition — SpherePacking.balls

## Statement

> [!definition] SpherePacking.balls
> Given a set $X \subset \mathbb{R}^d$ and a real number $r > 0$ (known as the *separation radius*) such that $\|x - y\| \geq r$ for all distinct $x, y \in X$, we define the *sphere packing* $\mathcal{P}(X)$ with centres at $X$ to be the union of all open balls of radius $r$ centred at points in $X$:
> 
> $$\mathcal{P}(X) := \bigcup_{x \in X} B_d(x, r)$$

**Used by**: [[e8packing]], [[lemma-inv-power-summable]], [[periodicspherepacking]], [[spherepacking]].

## Notes

> [!note]- Notes (click to expand)
> - The [[spherepackingdensity|density]] of $\mathcal{P}(X)$ is what the whole development is about, and [[spherepackingconstant|the constant]] $\Delta_d$ is its supremum over all $X$.
> - The separation radius is not part of the data in any essential way: [[spherepackingscale|scaling]] the centres by $c$ scales it by $c$ and leaves the density alone, so one may fix $r$ at any convenient value.
> - A packing invariant under a lattice is a [[periodicspherepacking|periodic packing]], and those are enough — [[thm-periodic-packing-optimal]] says the supremum over them is already $\Delta_d$.
