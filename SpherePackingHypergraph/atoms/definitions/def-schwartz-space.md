---
id: b8318af9fb58
type: definition
from: blueprint
lean:
  - SchwartzMap
formalized: true
---

# Definition — def:Schwartz-Space

## Statement

> [!definition] def:Schwartz-Space
> A $C^\infty$ function $f:\mathbb{R}^d\to\mathbb{C}$ is called a *Schwartz function* if it decays to zero as $\|x\|\to\infty$ faster then any inverse power of $\|x\|$, and the same holds for all partial derivatives of $f$, ie, if for all $k, n \in \mathbb{N}$, there exists a constant $C \in \mathbb{R}$ such that for all $x \in \mathbb{R}^d$, $\left\lVert x \right\rVert^k \cdot \left\lVert f^{(n)}(x) \right\rVert \leq C$, where $f^{(n)}$ denotes the $n$-th derivative of $f$ considered along with the appropriate operator norm. The set of all Schwartz functions from $\mathbb{R}^d$ to $\mathbb{C}$ is called the *Schwartz space*. It is an $\mathbb{R}$-vector space.

**Used by**: [[lemma-fourier-transform-is-automorphism]], [[lemma-schwartz-summable]], [[prop-a-schwartz]], [[prop-b-schwartz]].

## Notes

> [!note]- Notes (click to expand)
> - The point of the decay condition is that it survives the [[def-fourier-transform|Fourier transform]]: the space is carried onto itself, which is what lets [[thm-cohn-elkies-general]] impose conditions on $f$ and $\widehat f$ simultaneously.
> - Smoothness and rapid decay are dual to each other under the transform — derivatives become multiplication by polynomials and back — which is why both are required rather than either alone.
> - [[thm-smooth-fast-decay-schwartz]] is the criterion actually used: a radial function built from a one-variable function with the right decay lands here.
