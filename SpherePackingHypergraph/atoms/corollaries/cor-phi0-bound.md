---
id: 1e9b1a3eb8a7
type: corollary
---

# Corollary — cor:phi0-bound

## Statement

> [!corollary] cor:phi0-bound
> There exists a constant $C_0 > 0$ such that
> $$
> |\phi_0(z)| \le C_0 e^{-2 \pi \Im z}
> $$
> for all $z$ with $\Im z > 1/2$.

## Proof

> [!note]- Proof (click to expand)
> By Ramanujan's formula, $E_2 E_4 - E_6 = 3E_4' = 720 \sum_{n \ge 1} n \sigma_3(n) e^{2 \pi i n z}$ and
> 
> $$
> (E_2(z) E_4(z) - E_6(z))^{2} = 720^{2} e^{4 \pi i z} + O(e^{5 \pi i z}).
> $$
> 
> Then the result follows from Lemma~[[lemma-mod-div-disc-bound]] with $f(z) = (E_2 E_4 - E_6)^2$ and $n_0 = 4$.
