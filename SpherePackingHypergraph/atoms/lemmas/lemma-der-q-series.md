---
id: da8be44b7bb3
type: lemma
from: blueprint
lean:
  - D_qexp_tsum_pnat
formalized: true
---

# Lemma — lemma:der-q-series

## Statement

> [!lemma] lemma:der-q-series
> We have an equality of operators $D = q \frac{\mathrm{d}}{\mathrm{d} q}$. In particular, the $q$-series of the derivative of a quasimodular form $F(z) = \sum_{n \ge n_0} a_n q^n$ is $F'(z) = \sum_{n \ge n_0} n a_n q^n$.

## Proof

> [!note]- Proof (click to expand)
> Directly follows from the definition [[def-derivative]], where $\frac{1}{2 \pi i}\frac{\mathrm{d}}{\mathrm{d} z}e^{2\pi i n z} = n e^{2\pi i n z}$.
