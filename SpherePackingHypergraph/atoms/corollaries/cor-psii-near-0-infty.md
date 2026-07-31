---
id: 3f0a878be4ed
type: corollary
---

# Corollary — cor:psiI-near-0-infty

## Statement

> [!corollary] cor:psiI-near-0-infty
> We have
> $$
> \begin{aligned}
> \psi_I(it) &= O(t^2 e^{\pi/t}) \quad \text{as } t \to 0  \\
> \psi_I(it) &= O(e^{2 \pi t}) \quad \text{as } t \to \infty. 
> \end{aligned}
> $$

## Proof

> [!note]- Proof (click to expand)
> By [[eq-psis-define]], we have
> $$
> \psi_I(it) = (it)^{-2} \psi_S\left(\frac{-1}{it}\right) = -t^{-2} \psi_S\left(\frac{i}{t}\right).
> $$
> and combined with [[eq-psis-bound]] we get [[eq-psii-near-0]].
> [[eq-psii-near-infty]] follows from Lemma [[lemma-psi-bound]].
