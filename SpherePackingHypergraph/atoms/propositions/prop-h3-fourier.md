---
id: d125f456fa83
type: proposition
from: blueprint
---

# Proposition — prop:H3-fourier

## Statement

> [!proposition] prop:H3-fourier
> $H_3$ admits a Fourier series of the form
> $$
> H_3(z) = \sum_{n \ge 0} c_{H_3}(n) e^{\pi i n z}
> $$
> for some $c_{H_3}(n) \in \mathbb{R}_{\ge 0}$ with $c_{H_3}(0) = 1$ and $c_{H_3}(n) = O(n^k)$ for some $k \in \mathbb{N}$.
> Especially, $H_3$ is not cuspidal.

## Proof

> [!note]- Proof (click to expand)
> We have
> $$
> H_3(z) = \Theta_3(z)^{4} = \left(\sum_{n \in \mathbb{Z}} e^{\pi i n^2 z}\right)^{4} = \left(1 + 2 \sum_{n \ge 1} e^{\pi i n^2 z}\right)^{4} = 1 + O(e^{\pi i z}).
> $$
