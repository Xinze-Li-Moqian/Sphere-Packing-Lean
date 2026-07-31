---
id: c82a212ab0ec
type: theorem
lean:
  - SchwartzMap.PoissonSummation_Lattices
formalized: true
---

# Theorem — Poisson summation formula

## Statement

> [!theorem] Poisson summation formula
> Let $\Lambda$ be a lattice in $\mathbb{R}^d$, and let $f:\mathbb{R}^d\to\mathbb{R}$ be a Schwartz function. Then, for all $v \in \mathbb{R}^d$,
> 
> $$\sum_{\ell\in\Lambda}f(\ell + v) = \frac{1}{\operatorname{Vol}\!\left(\mathbb{R}^d/\Lambda\right)} \sum_{m\in\Lambda^*}\widehat{f}(m) e^{-2\pi i \left\langle v, m \right\rangle}.$$

## Proof

> [!note]- Proof (click to expand)
> One possible proof would be by induction on $d$. However, there are numerous nuances involved, particularly in manipulating nested infinite sums. Ideas would be appreciated.
