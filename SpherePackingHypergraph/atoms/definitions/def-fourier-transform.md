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

**Used by**: [[eq-a-fourier]], [[eq-b-fourier]], [[eq-cohn-elkies-condition-2]], [[eq-g2]].

## Notes

> [!note]- Notes (click to expand)
> - Defined here for $L^1$, but the object it is used on is the [[def-schwartz-space|Schwartz space]], where it is an automorphism — [[lemma-fourier-transform-is-automorphism]] — and where the inversion formula needs no qualification.
> - The whole method rests on Poisson summation, which trades a sum of $f$ over a [[iszlattice|lattice]] for a sum of $\widehat f$ over its [[def-dual-lattice|dual]]. That is why the [[thm-cohn-elkies-general|linear programming bound]] constrains $f$ and $\widehat f$ at once, and why self-duality of $\Lambda_8$ is the coincidence the proof turns on.
> - The two functions the proof finally exhibits are eigenfunctions of this operator: [[def-a-definition|$a_{\mathrm{rad}}$]] with eigenvalue $+1$ and [[def-b-definition|$b_{\mathrm{rad}}$]] with eigenvalue $-1$.
