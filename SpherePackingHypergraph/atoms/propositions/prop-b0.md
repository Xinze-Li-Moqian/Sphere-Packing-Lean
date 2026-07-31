---
id: bff53b85e524
type: proposition
lean:
  - MagicFunction.b.SpecialValues.b_zero
formalized: true
---

# Proposition — prop:b0

## Statement

> [!proposition] prop:b0
> We have $b(0) = 0$.

**Used by**: [[thm-g1]].

## Proof

> [!note]- Proof (click to expand)
> Let $r\to0^+$ in [[prop-b-another-integral]]. Here, unlike [[prop-a0]], the bracket has no $r^{-4}$ pole — its strongest singularity is $\frac{144}{\pi r^2}$ — so the prefactor wins:
> $$b(0)=\lim_{r\to0}4i\,\sin^2\!\big(\tfrac{\pi r^2}{2}\big)\Big(\frac{144}{\pi r^2}+\frac{1}{\pi(r^2-2)}+\int_0^\infty\!\big(\psi_I(it)-144-e^{2\pi t}\big)e^{-\pi r^2t}dt\Big)=0,$$
> each term being $O(r^{4})\cdot O(r^{-2})=O(r^2)$ or better. The integral converges absolutely because $\psi_I(it)-144-e^{2\pi t}=O(e^{-\pi t})$ as $t\to\infty$ ([[lemma-psii-psit-psis-fourier]]) and $\psi_I(it)=O(t^2e^{-\pi/t})$ as $t\to0$ ([[eq-psii-near-0]]).
>
> $b(0)=0$ is forced structurally as well: $b$ is a $-1$ eigenfunction of the [[def-fourier-transform|Fourier transform]] ([[prop-b-fourier]]), and at the origin $b(0)=\widehat b(0)=-b(0)$.

**Uses**: [[prop-b-another-integral]].
