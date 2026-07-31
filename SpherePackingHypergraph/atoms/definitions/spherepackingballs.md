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
