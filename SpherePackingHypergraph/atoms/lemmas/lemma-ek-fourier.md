---
id: 044af3957846
type: lemma
from: blueprint
lean:
  - E_k_q_expansion
formalized: true
---

# Lemma — lemma:Ek-Fourier

## Statement

> [!lemma] lemma:Ek-Fourier
> The [[def-ek|Eisenstein series]] possesses the Fourier expansion
> $$E_k(z)=1+\frac{2}{\zeta(1-k)}\sum_{n=1}^\infty \sigma_{k-1}(n)\,e^{2\pi i z}, $$
> where $\sigma_{k-1}(n)\,=\,\sum_{d|n} d^{k-1}$. In particular, we have
> $$
> \begin{aligned}
> E_4(z)\,=\,& 1+240\sum_{n=1}^\infty \sigma_3(n)\,e^{2\pi i n z} \notag \\
> E_6(z)\,=\,& 1-504\sum_{n=1}^\infty \sigma_5(n)\,e^{2\pi i n z}. \notag
> \end{aligned}
> $$

## Proof

> [!note]- Proof (click to expand)
> 

**Uses**: [[def-ek]].
