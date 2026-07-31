---
id: 31459b05836d
type: lemma
from: blueprint
---

# Lemma — lemma:psi-bound

## Statement

> [!lemma] lemma:psi-bound
> There exist constants $C_I, C_S, C_T > 0$ such that
> $$
> \begin{aligned}
> |\psi_I(z)| &\le C_I e^{2\pi \Im z},  \\
> |\psi_T(z)| &\le C_T e^{2\pi \Im z},  \\
> |\psi_S(z)| &\le C_S e^{- \pi \Im z} 
> \end{aligned}
> $$

**In terms of**: [[def-psii-psit-psis]].

## Proof

> [!note]- Proof (click to expand)
> The proof is similar to that of Lemma [[cor-phi0-bound]], follows from Lemma [[lemma-mod-div-disc-bound]] and the fact that the vanishing orders of the numerators of $\psi_I$, $\psi_T$, and $\psi_S$ at infinity are $0$, $0$ (i.e. not [[def-cusp-form|cusp forms]]), and $\frac{3}{2}$ respectively.
