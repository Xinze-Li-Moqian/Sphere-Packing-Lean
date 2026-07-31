---
id: f3d45a3596a4
type: corollary
from: blueprint
formalized: true
---

# Corollary — cor:MLDE-pos

## Statement

> [!corollary] cor:MLDE-pos
> [[eq-ddf]] (resp. [[eq-ddg]]) is positive (resp. negative) on the (positive) imaginary axis.

## Proof

> [!note]- Proof (click to expand)
> From [[eq-e2]] and Lemma [[cor-disc-pos]],
> 
> $$
> 7200 (-E_2'(it)) \Delta(it) = 7200 \cdot 24 \left(\sum_{n \ge 1} n \sigma_1(n) e^{-2 \pi n t}\right) \cdot \Delta(it) > 0.
> $$
> 
> Negativity of [[eq-ddg]], i.e. $-640 \Delta(it) H_2(it) < 0$ follows from Corollary [[cor-theta-pos]] and [[cor-disc-pos]].

**Uses**: [[cor-disc-pos]], [[cor-theta-pos]], [[def-e2]], [[lemma-fg-de]].
