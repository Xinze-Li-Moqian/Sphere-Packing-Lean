---
id: 2fc0db19941f
type: corollary
---

# Corollary — cor:phi0-near-0-infty

## Statement

> [!corollary] cor:phi0-near-0-infty
> We have
> $$
> \begin{aligned}
> \phi_0\left(\frac{i}{t}\right) &= O(e^{-2 \pi / t}) \quad \text{as } t \to 0  \\
> \phi_0\left(\frac{i}{t}\right) &= O(t^{-2}e^{2 \pi t}) \quad \text{as } t \to \infty.  \\
> \end{aligned}
> $$

## Proof

> [!note]- Proof (click to expand)
> The first estimate follows from [[eq-phi0-bound]] with $z = i/t$.
> For the second estimate, by [[eq-phi0-trans-s]], [[eq-phi2-bound]], and [[eq-phi4-bound]], we have
> $$
> \left|\phi_0\left(\frac{i}{t}\right)\right| \le |\phi_0(it)| + \frac{12}{\pi t} |\phi_{-2}(it)| + \frac{36}{\pi^2 t^2} |\phi_{-4}(it)|
> \le C_0 e^{-2 \pi t} + \frac{12}{\pi t} \cdot C_{-2} + \frac{36}{\pi^2 t^2} \cdot C_{-4} e^{2 \pi t} = O(t^{-2}e^{2 \pi t}).
> $$
