---
id: 3b4b07db5a1b
type: lemma
from: blueprint
---

# Lemma — lemma:Schwartz-summable

## Statement

> [!lemma] lemma:Schwartz-summable
> Let $f : \mathbb{R}^d \to \mathbb{C}$ be a [[def-schwartz-space|Schwartz function]] and let $X \subset \mathbb{R}^d$ be [[periodicspherepacking|periodic]] with respect to some [[iszlattice|lattice]] $\Lambda \subset \mathbb{R}^d$. Then,
> 
> $$\sum_{x \in X} |f(x)| < \infty.$$

## Proof

> [!note]- Proof (click to expand)
> Without loss of generality, assume that $0 \notin X$: if $0 \in X$, then we can add the $f(0)$ term to the sum over nonzero elements of $X$, which, if the sum over the nonzero elements converges absolutely, will be equal to the sum over all of $X$. Now, we know that for all $k \in \mathbb{N}$, there exists some constant $C$ such that $|f(x)| \leq C\left\lVert x \right\rVert^{-k}$ for all $x \in \mathbb{R}^d$. Choosing $k$ to be sufficiently large, we see that
> 
> $$\sum_{x \in X} |f(x)| \leq \sum_{x \in X} \frac{C}{\left\lVert x \right\rVert^{k}} = C \sum_{x \in X} \frac{1}{\left\lVert x \right\rVert^k} < \infty.$$
