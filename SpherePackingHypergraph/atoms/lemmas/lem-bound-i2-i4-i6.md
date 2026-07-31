---
id: 04ed548f1041
type: lemma
from: blueprint
---

# Lemma — lem:bound-I2-I4-I6

## Statement

> [!lemma] lem:bound-I2-I4-I6
> There exist $C_1, C_2 > 0$ such that for all $r \geq 0$,
> $$
> |I_2(r)|, |I_4(r)| \leq C_1 e^{-\pi r}
> $$
> and
> $$
> |I_6(r)| \leq C_2 \frac{e^{-\pi(r + 2)}}{r + 2}
> $$

## Proof

> [!note]- Proof (click to expand)
> For $I_2(r)$, parametrize $z$ as $z = t + i$ for $t \in [-1,0]$, and we have
> $$
> I_2(r) = \int_{-1}^0 \phi_0\left(\frac{-1}{t + 1 + i}\right) (t + 1 + i)^2 e^{\pi i r t} e^{-\pi r} \, \mathrm{d} t.
> $$
> Since the function $z \mapsto \phi_0\left(\frac{-1}{z+1}\right) (z+1)^2$ is holomorphic and bounded on the contour,
> there exists $C > 0$ such that $|\phi_0\left(\frac{-1}{z+1}\right) (z + 1)^2| \leq C$, and the absolute value of the integral can be bounded by
> $$
> |I_2(r)| \le \int_{-1}^{0} C e^{-\pi r} \, \mathrm{d} t = C e^{-\pi r}.
> $$
> The bound for $I_4(r)$ is similar.
> For $I_6(r)$, parametrize $z$ as $z = i t$ for $t \in [1, \infty)$, and we have
> $$
> I_6(r) = 2 i \int_1^{\infty} \phi_0(i t) e^{-\pi r t} \, \mathrm{d} t
> $$
> and the absolute value can be bounded as (using Corollary [[cor-phi0-bound]])
> $$
> |I_6(r)| \leq 2 \int_1^{\infty} |\phi_0(i t)| e^{-\pi r t} \, \mathrm{d} t \leq \frac{2C_0}{\pi} \int_1^{\infty} e^{-2\pi t} e^{-\pi r t} \, \mathrm{d} t = \frac{2C_0}{\pi} \frac{e^{-\pi (r + 2)}}{r + 2}.
> $$
