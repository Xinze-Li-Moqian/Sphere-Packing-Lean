---
id: 65a0e84d04e7
type: lemma
from: blueprint
---

# Lemma — lemma:log-der-inf

## Statement

> [!lemma] lemma:log-der-inf
> Let $F$ be a quasimodular form where the vanishing order of $F$ at infinity is $n_0 > 0$, i.e. $F(z) = \sum_{n \geq n_0} a_n q^{n}$ with $a_{n_0} \ne 0$. Then
> $$
> \lim_{t \to \infty} \frac{F'(it)}{F(it)} = n_0.
> $$

## Proof

> [!note]- Proof (click to expand)
> By Lemma [[lemma-der-q-series]],
> $$
> \lim_{t \to \infty} \frac{F'(it)}{F(it)} = \lim_{t \to \infty} \frac{\sum_{n \ge n_0} n a_n e^{-2 \pi n t}}{\sum_{n \ge n_0} a_n e^{-2 \pi n t}} = \lim_{t \to \infty} \frac{n_0 a_{n_0} e^{-2 \pi n_0 t} + O(e^{-2 \pi (n_0 + 1) t})}{a_{n_0} e^{-2 \pi n_0 t} + O(e^{-2 \pi (n_0 + 1) t})} = n_0.
> $$
