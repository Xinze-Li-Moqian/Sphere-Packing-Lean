---
id: 4b0f9e2d1c73
type: definition
---

# Definition — cusp form

Written here, not imported. The blueprint uses "cusp form" six times — the
$-1$ eigenfunction is built from one, and `thm:anti-serre-der-pos` is stated
about one — and defines it nowhere, so every statement resting on it named a
concept the pool could not reach.

## Statement

> [!definition] cusp form
> Let $\Gamma$ be a [[def-congruence-subgroup|congruence subgroup]] and let $f \in M_k(\Gamma)$ be a [[def-mk|modular form]] of weight $k$. Then $f$ is a *cusp form* if it vanishes at every cusp of $\Gamma$: for every $\gamma \in \Gamma_1$,
> $$
> \lim_{\operatorname{Im} z \to \infty} (f\vert_k\gamma)(z) = 0 .
> $$
> Equivalently, the constant term of the $q$-expansion of $f\vert_k\gamma$ is zero for every such $\gamma$. The cusp forms of weight $k$ and level $\Gamma$ form a subspace $S_k(\Gamma) \subseteq M_k(\Gamma)$.

## Notes

> [!note]- Notes (click to expand)
> - A [[def-mk|modular form]] is required only to be *holomorphic* at the cusps — bounded as $\operatorname{Im} z \to \infty$. A cusp form is the stronger condition, and the gap between the two is exactly the constant term.
> - Vanishing has to be checked after applying the [[def-slash-operator|slash operator]] by each $\gamma$, because a group with several cusps reaches them by translating $i\infty$ around; for level one there is a single cusp and the condition is that one limit.
> - The [[def-disc-definition|discriminant form]] $\Delta$ is the first example in level one, and the smallest weight in which a nonzero cusp form exists is $k = 12$ — which is why the dimension counts in this development start where they do.
