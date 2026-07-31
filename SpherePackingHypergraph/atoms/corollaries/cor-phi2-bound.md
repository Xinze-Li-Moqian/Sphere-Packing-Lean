---
id: e1cff58ec47d
type: corollary
---

# Corollary — cor:phi2-bound

## Statement

> [!corollary] cor:phi2-bound
> There exists a constant $C_{-2} > 0$ such that
> $$
> |\phi_{-2}(z)| \le C_{-2}
> $$
> for all $z$ with $\Im z > 1/2$.

## Proof

> [!note]- Proof (click to expand)
> By [[def-phi4-phi2-phi0|the definition]], $\phi_{-2}=E_4(E_2E_4-E_6)/\Delta$. By [[thm-ramanujan-formula]], $E_2E_4-E_6=3E_4^{\prime}=720\sum_{n\ge1}n\sigma_3(n)q^n$: the numerator has no constant term. The denominator $\Delta=q\prod_{n\ge1}(1-q^n)^{24}$ ([[def-disc-definition]]) starts at $q$ as well and never vanishes on $\mathfrak{H}$ ([[cor-disc-nonvanishing]]).
>
> So $\phi_{-2}$ is holomorphic on $\mathfrak{H}$, $1$-periodic, and its $q$-expansion $E_4\cdot 3E_4^{\prime}/\Delta$ has only nonnegative powers of $q$ — the $q$ upstairs cancels the $q$ downstairs. A $1$-periodic holomorphic function whose expansion has no negative powers is bounded on $\Im z\ge 1/2$: the expansion converges absolutely at $q_0=e^{-\pi}$ and dominates uniformly beyond. Hence $|\phi_{-2}(z)|\le C_{-2}$ there.
>
> The same argument gives the neighbouring bounds: one factor of $E_2E_4-E_6$ is what separates this from [[cor-phi4-bound]], and two from [[cor-phi0-bound]].

**Uses**: [[def-phi4-phi2-phi0]], [[lemma-ek-fourier]], [[lemma-mod-div-disc-bound]].
