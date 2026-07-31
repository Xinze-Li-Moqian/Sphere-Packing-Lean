---
id: f74ffa0a44c8
type: corollary
from: blueprint
lean:
  - Δ_imag_axis_pos
formalized: true
---

# Corollary — cor:disc-pos

## Statement

> [!corollary] cor:disc-pos
> $\Delta(it) > 0$ for all $t > 0$.

## Proof

> [!note]- Proof (click to expand)
> By [[def-disc-definition]], we have
> $$
> \Delta(it) = e^{-2 \pi t} \prod_{n \ge 1} (1 - e^{-2 \pi n t})^{24} > 0.
> $$
