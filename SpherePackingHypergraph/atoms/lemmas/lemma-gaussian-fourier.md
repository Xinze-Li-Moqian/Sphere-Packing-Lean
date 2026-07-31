---
id: aa120795e725
type: lemma
---

# Lemma — lemma:Gaussian-Fourier

## Statement

> [!lemma] lemma:Gaussian-Fourier
> $$
> \mathcal{F}(e^{\pi i \|x\|^2 z})(y) = z^{-4}\,e^{\pi i \|y\|^2 \,(\frac{-1}{z}) }.
> $$

**In terms of**: [[def-fourier-transform]].

## Proof

> [!note]- Proof (click to expand)
> Both sides are holomorphic in $z$ on the upper half-plane and agree on the imaginary axis; that is the whole proof.
>
> **On the imaginary axis.** For $z=it$, $t>0$, the claim is the classical Gaussian identity. In one variable, completing the square and shifting the contour gives $\int_\mathbb{R} e^{-\pi t x^2}e^{-2\pi i xy}\,dx=t^{-1/2}e^{-\pi y^2/t}$, and the eight-dimensional integral factors as a product of eight such, so by [[def-fourier-transform|the definition]]
> $$\mathcal{F}\big(e^{-\pi t\|x\|^2}\big)(y)=t^{-4}\,e^{-\pi\|y\|^2/t}.$$
> This is the claimed identity at $z=it$: there $z^{-4}=(it)^{-4}=t^{-4}$ and $e^{\pi i\|y\|^2(-1/z)}=e^{-\pi\|y\|^2/t}$.
>
> **Analytic continuation.** Fix $y$. The left side is holomorphic in $z\in\mathfrak{H}$: the integrand $e^{\pi i\|x\|^2 z}$ is dominated by $e^{-\pi\|x\|^2\,\Im z}$, locally uniformly, so differentiation under the integral is justified. The right side is holomorphic on $\mathfrak{H}$ as well — and $z^{-4}$ needs no branch choice, because the exponent is the even integer $d/2=4$: this is where dimension $8$ enters, as $(z/i)^{-d/2}=z^{-4}i^{4}=z^{-4}$ exactly when $d\equiv 0\pmod 8$. Two holomorphic functions agreeing on the ray $i\mathbb{R}_{>0}$ agree on all of $\mathfrak{H}$ by the identity theorem.
>
> This is equation (36) of [[ref-via2017]]; the family $z\mapsto e^{\pi i\|x\|^2 z}$ is the bridge on which the [[def-fourier-transform|Fourier transform]] acts by $z\mapsto -1/z$, i.e. by the generator $S$ ([[def-gamma-generators]]).

**Uses**: [[def-fourier-transform]].
