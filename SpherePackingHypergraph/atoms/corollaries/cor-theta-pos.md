---
id: 34a4429087a4
type: corollary
from: blueprint
lean:
  - H₂_imag_axis_pos
  - H₄_imag_axis_pos
---

# Corollary — cor:theta-pos

## Statement

> [!corollary] cor:theta-pos
> $H_2(it)$ and $H_4(it)$ are positive for $t > 0$.

**In terms of**: [[def-h2-h3-h4]].

## Proof

> [!note]- Proof (click to expand)
> By the transformation law [[eq-h2-transform-s]], it is enough to prove the positivity for $\Theta_2(it)$, which is clear from its definition:
> $$
> \Theta_{2}(it) = \sum_{n \in \mathbb{Z}} e^{- \pi (n + \frac{1}{2})^{2} t} > 0.
> $$

**Uses**: [[lemma-theta-transform-s-t]].
