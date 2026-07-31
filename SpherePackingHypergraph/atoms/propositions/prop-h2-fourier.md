---
id: 18c298170f0f
type: proposition
from: blueprint
---

# Proposition — prop:H2-fourier

## Statement

> [!proposition] prop:H2-fourier
> $H_2$ admits a Fourier series of the form
> $$
> H_2(z) = \sum_{n \ge 1} c_{H_2}(n) e^{\pi i n z}
> $$
> for some $c_{H_2}(n) \in \mathbb{R}_{\ge 0}$, with $c_{H_2}(1) = 16$ and $c_{H_2}(n) = O(n^k)$ for some $k \in \mathbb{N}$.

**In terms of**: [[def-h2-h3-h4]].

## Proof

> [!note]- Proof (click to expand)
> We have
> $$
> \begin{aligned}
> H_2(z) &= \Theta_2(z)^4 \\
> &= \left(\sum_{n \in \mathbb{Z}} e^{\pi i (n + \frac{1}{2})^{2} z}\right)^{4} \\
> &= \left(2\sum_{n \ge 0} e^{\pi i (n + \frac{1}{2})^{2} z}\right)^{4} \\
> &= \left(2 e^{\pi i z / 4} + 2 \sum_{n \ge 1} e^{\pi i (n^2 + n + \frac{1}{4}) z}\right)^{4} \\
> &= 16 e^{\pi i z}\left(1 + \sum_{n \ge 1} e^{\pi i (n^2 + n)z}\right)^{4} \\
> &= 16 e^{\pi i z} + \sum_{n \ge 2} c_{H_2}(n) e^{\pi i n z} \\
> &= \sum_{n \ge 1} c_{H_2}(n) e^{\pi i n z}.
> \end{aligned}
> $$

**Uses**: [[def-h2-h3-h4]].
