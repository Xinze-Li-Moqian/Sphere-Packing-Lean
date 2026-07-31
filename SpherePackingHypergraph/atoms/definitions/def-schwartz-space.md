---
id: b8318af9fb58
type: definition
lean:
  - SchwartzMap
formalized: true
---

# Definition — def:Schwartz-Space

## Statement

> [!definition] def:Schwartz-Space
> A $C^\infty$ function $f:\mathbb{R}^d\to\mathbb{C}$ is called a *Schwartz function* if it decays to zero as $\|x\|\to\infty$ faster then any inverse power of $\|x\|$, and the same holds for all partial derivatives of $f$, ie, if for all $k, n \in \mathbb{N}$, there exists a constant $C \in \mathbb{R}$ such that for all $x \in \mathbb{R}^d$, $\left\lVert x \right\rVert^k \cdot \left\lVert f^{(n)}(x) \right\rVert \leq C$, where $f^{(n)}$ denotes the $n$-th derivative of $f$ considered along with the appropriate operator norm. The set of all Schwartz functions from $\mathbb{R}^d$ to $\mathbb{C}$ is called the *Schwartz space*. It is an $\mathbb{R}$-vector space.
