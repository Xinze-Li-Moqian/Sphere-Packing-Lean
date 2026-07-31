---
id: 26d62c2c1e7c
type: definition
from: blueprint
lean:
  - FourierTransform.fourier
formalized: true
---

# Definition — def:Fourier-Transform

## Statement

> [!definition] def:Fourier-Transform
> The Fourier transform of an $L^1$-function $f:\mathbb{R}^d\to\mathbb{C}$ is defined as
> 
> $$\mathcal{F}(f)(y) = \widehat{f}(y) := \int_{\mathbb{R}^d} f(x)e^{-2\pi i \langle x, y \rangle} \,\mathrm{d}x, \quad y \in \mathbb{R}^d$$
> 
> where $\langle x, y \rangle = \frac12\|x\|^2 + \frac12\|y\|^2 - \frac12\|x - y\|^2$ is the standard scalar product in $\mathbb{R}^d$.
