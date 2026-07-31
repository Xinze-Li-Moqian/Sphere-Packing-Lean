---
id: 4e143fd3c98e
type: lemma
from: blueprint
---

# Lemma — lem:integral-bound

## Statement

> [!lemma] lem:integral-bound
> For all $n \in \mathbb{N}$, there exists a constant $C'$ such that for all $r \geq 0$,
> $$
> \begin{aligned}
> r^n \cdot \int_{1}^{\infty} e^{-2\pi s} \, e^{-\pi r /s} \, \mathrm{d} s \leq C'
> \end{aligned}
> $$

**Used by**: [[prop-a-schwartz]].

## Proof

> [!note]- Proof (click to expand)
> Fix $n \in \mathbb{N}$. We know there exists a constant $C$ such that for all $x \geq 0$, $\left\lvert x \right\rvert^n \cdot \left\lvert e^{-\pi x} \right\rvert \leq C$. In particular, for all $r \geq 0$ and $s \geq 1$, $r^n \cdot e^{-\pi r/s} \leq C s^n$. Hence, for all $r \in \mathbb{R}$, we can write
> $$
> \begin{aligned}
> r^n \cdot \int_{1}^{\infty} e^{-2\pi s} \, e^{-\pi r /s} \, \mathrm{d}{s}
> = \int_{1}^{\infty} e^{-2\pi s} \, \left(\left\lvert r \right\rvert^n \cdot e^{-\pi r /s}\right) \, \mathrm{d}{s}
> \leq C \int_{1}^{\infty} e^{-2\pi s} \, s^n \, \mathrm{d}{s}
> \end{aligned}
> $$
> 
> The $\Gamma$ function is given by
> $$
> \begin{aligned}
> \Gamma(x) = \int_{0}^{\infty} e^{-u} \, u^{x-1} \, \mathrm{d}{u}
> \end{aligned}
> $$
> for all $x > 0$. Hence, writing $u = 2\pi s$ and using $\Gamma(n+1) = n!$, we get
> 
> $$
> \begin{aligned}
> C \int_{1}^{\infty} e^{-2\pi s} \, s^n \, \mathrm{d}{s}
> \leq C \int_{0}^{\infty} e^{-2\pi s} \, s^n \, \mathrm{d}{s}
> = C \int_{0}^{\infty} \frac{1}{(2\pi)^{n+1}} e^{-u} \, u^n \, \mathrm{d}{u}
> = \frac{C}{(2\pi)^n} \Gamma(n+1)
> = \frac{C \cdot n!}{(2\pi)^n}
> \end{aligned}
> $$
> Defining $C' := \frac{C \cdot n!}{(2\pi)^n}$ finishes the proof.
