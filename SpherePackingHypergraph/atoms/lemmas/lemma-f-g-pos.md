---
id: a1fd01d39c33
type: lemma
lean:
  - F_imag_axis_pos
  - G_imag_axis_pos
formalized: true
---

# Lemma — lemma:F-G-pos

## Statement

> [!lemma] lemma:F-G-pos
> For all $t > 0$, we have $F(it) > 0$ and $G(it) > 0$.

## Proof

> [!note]- Proof (click to expand)
> By Ramanujan's identity [[eq-de4]], we have $F(z) = 9 E_4'(z)^2$ and
> $$
> F(it) = 9E_4'(it)^2 = 9 \left(240\sum_{n \geq 1} n \sigma_3(n) e^{-2 \pi n t} \right)^{2} > 0.
> $$
> $G(it) > 0$ follows from positivity of $H_2(it)$ and $H_4(it)$ (Lemma [[cor-theta-pos]]).
