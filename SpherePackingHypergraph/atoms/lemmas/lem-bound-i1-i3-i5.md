---
id: afdb3c98371f
type: lemma
---

# Lemma — lem:bound-I1-I3-I5

## Statement

> [!lemma] lem:bound-I1-I3-I5
> There exists $C > 0$ such that for all $r \geq 0$,
> $$
> |I_1(r)|, |I_3(r)|, |I_5(r)| \leq C \int_1^{\infty} e^{-2\pi s} \, e^{-\pi r / s} \, \mathrm{d} s.
> $$

## Proof

> [!note]- Proof (click to expand)
> We only prove the bound for $I_1(r)$, as the other two are similar.
> By the change of variable $z = -1 + i t$ for $t \in [0,1]$, we have
> $$
> I_1(r) = -i \int_0^1 \phi_0\left(\frac{-1}{i t}\right) t^2 e^{-\pi i r} \cdot e^{-\pi r t} \, \mathrm{d} t.
> $$
> With the change of variable $s = 1 / t$, we get
> $$
> I_1(r) = i \int_1^{\infty} \phi_0(i s) \cdot s^{-4} \cdot e^{-\pi i r} \cdot e^{-\pi r / s} \, \mathrm{d} s
> $$
> and the absolute value can be bounded as
> $$
> |I_1(r)| \leq \int_1^{\infty} |\phi_0(i s)| \cdot s^{-4} \cdot |e^{-\pi i r}| \cdot e^{-\pi r / s} \, \mathrm{d} s \le \int_1^{\infty} |\phi_0(is)| \cdot e^{-\pi r / s} \, \mathrm{d} s.
> $$
> Now, Corollary [[cor-phi0-bound]] shows
> $$
> |I_1(r)| \leq C_0 \int_1^{\infty} e^{-2\pi s} \, e^{-\pi r / s} \, \mathrm{d} s.
> $$
