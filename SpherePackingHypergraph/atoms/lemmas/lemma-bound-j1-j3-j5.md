---
id: 716c68f6b9a6
type: lemma
---

# Lemma — lemma:bound-J1-J3-J5

## Statement

> [!lemma] lemma:bound-J1-J3-J5
> There exist a constant $C > 0$ such that
> $$
> \begin{aligned}
> |J_1(r)|, |J_3(r)|, |J_5(r)| &\le C \int_1^{\infty} e^{-\pi s} e^{\pi r / s}\, \mathrm{d} s.
> \end{aligned}
> $$

**In terms of**: [[def-b-definition]].

## Proof

> [!note]- Proof (click to expand)
> All three integrals live where $\Im z$ is small, so the point is to control $\psi$ near the real axis by its behaviour near $i\infty$, through the $S$-transform.
>
> **A bound on $\psi_I$ low down.** From [[def-psii-psit-psis]], $\psi_S=\psi_I|_{-2}S$, i.e. $\psi_S(z)=z^2\psi_I(-1/z)$; hence $\psi_I(is)=-s^2\,\psi_S(i/s)$ for $s>0$. For $s\le 1$, $\Im(i/s)\ge1$, where [[lemma-psi-bound]] gives $|\psi_S(w)|\le C_S e^{-\pi\Im w}$; so
> $$|\psi_I(is)|\;\le\;C_S\,s^2\,e^{-\pi/s},\qquad 0<s\le1,$$
> which is the estimate recorded as [[eq-psii-near-0]].
>
> **$J_5$.** By [[def-b-definition]], $J_5(r)=-2\int_0^i\psi_I(z)e^{\pi irz}dz$; on $z=is$, $|e^{\pi ir\,(is)}|=e^{-\pi rs}\le1$ for $r\ge0$ (the case used, since $r=\|x\|^2$). So $|J_5(r)|\le 2C_S\int_0^1 s^2e^{-\pi/s}e^{-\pi rs}\,ds$; substituting $s=1/u$, $ds=du/u^2$, this is $2C_S\int_1^\infty u^{-4}e^{-\pi u}e^{-\pi r/u}\,du\le 2C_S\int_1^\infty e^{-\pi u}\,e^{\pi r/u}\,du$.
>
> **$J_1$ and $J_3$.** $\psi_T=\psi_I|_{-2}T$ and $T$ carries no automorphy factor, so $\psi_T(z)=\psi_I(z+1)$; and $\psi_I$ has period $2$, since by [[lemma-psi-new]] it is a rational expression in $H_2,H_4$, which are power series in $e^{\pi iz}$. Hence on the two vertical segments $\psi_T(-1+is)=\psi_I(is)$ and $\psi_T(1+is)=\psi_I(2+is)=\psi_I(is)$. With $|e^{\pi ir(\pm1+is)}|=e^{-\pi rs}$, both integrals obey the same bound as $J_5$ (without even the factor $2$).
>
> Taking $C=2C_S$ covers all three. The derivation gives the stronger $e^{-\pi r/s}$ in place of $e^{\pi r/s}$; the stated form follows a fortiori for $r\ge 0$.
