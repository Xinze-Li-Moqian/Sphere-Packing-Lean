---
id: 014223bd98e3
type: corollary
---

# Corollary — cor:phi4-bound

## Statement

> [!corollary] cor:phi4-bound
> There exists a constant $C_{-4} > 0$ such that
> $$
> |\phi_{-4}(z)| \le C_{-4} e^{2 \pi \Im z}
> $$
> for all $z$ with $\Im z > 1/2$.

## Proof

> [!note]- Proof (click to expand)
> By [[def-phi4-phi2-phi0|the definition]], $\phi_{-4}=E_4^2/\Delta$. The numerator has constant term $1$; the denominator $\Delta=q\prod(1-q^n)^{24}$ ([[def-disc-definition]]) starts at $q$ and never vanishes on $\mathfrak{H}$ ([[cor-disc-nonvanishing]]). So the $q$-expansion of $\phi_{-4}$ begins at $q^{-1}$:
> $$\phi_{-4}(z)=q^{-1}+O(1),\qquad q=e^{2\pi iz}.$$
> On $\Im z>1/2$ the tail is uniformly bounded (absolute convergence at $q_0=e^{-\pi}$, as in [[cor-phi2-bound]]), and $|q^{-1}|=e^{2\pi\Im z}$, so $|\phi_{-4}(z)|\le C_{-4}\,e^{2\pi\Im z}$.
>
> The single pole at the cusp is the point: $\phi_{-4}$ grows exactly like one power of $q^{-1}$, which is what the contour estimates in [[prop-a-schwartz]] absorb.

**Uses**: [[def-phi4-phi2-phi0]], [[lemma-ek-fourier]], [[lemma-mod-div-disc-bound]].
