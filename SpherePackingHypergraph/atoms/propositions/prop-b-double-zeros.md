---
id: d3392155fab3
type: proposition
from: blueprint
---

# Proposition — prop:b-double-zeros

## Statement

> [!proposition] prop:b-double-zeros
> For $r>\sqrt{2}$ function $b(r)$ can be expressed as
> $$
> b(r)=-4\sin(\pi r^2/2)^2\,\int\limits_{0}^{i\infty}\psi_I(z)\,e^{\pi i r^2 \,z}\,dz.
> $$

## Proof

> [!note]- Proof (click to expand)
> We denote the right hand side of [[eq-b-double-zeroes]] by $c(r)$.
> By Corollary [[cor-psii-near-0-infty]], the integral in [[eq-b-double-zeroes]] converges for $r>\sqrt{2}$.
> Then we rewrite it in the following way:
> $$c(r)=\int\limits_{-1}^{i\infty-1}\psi_I(z+1)\,e^{\pi i r^2 \,z}\,dz-2\int\limits_{0}^{i\infty}\psi_I(z)\,e^{\pi i r^2 \,z}\,dz+
> \int\limits_{1}^{i\infty+1}\psi_I(z-1)\,e^{\pi i r^2 \,z}\,dz.$$
> From the Fourier expansion [[eq-psi-fourier-i]] we know that $\psi_I(z)=e^{-2\pi i z}+O(1)$ as $\Im(z)\to\infty$.
> By assumption $r^2>2$, hence we can deform the path of integration and write
> $$
> \begin{aligned}
> \int\limits_{-1}^{i\infty-1}\psi_I(z+1)\,e^{\pi i r^2 \,z}\,dz=&
> \int\limits_{-1}^{i}\psi_T(z)\,e^{\pi i r^2 \,z}\,dz+\int\limits_{i}^{i\infty}\psi_T(z)\,e^{\pi i r^2 \,z}\,dz\\
> \int\limits_{1}^{i\infty+1}\psi_I(z-1)\,e^{\pi i r^2 \,z}\,dz=&
> \int\limits_{-1}^{i}\psi_T(z)\,e^{\pi i r^2 \,z}\,dz+\int\limits_{i}^{i\infty}\psi_T(z)\,e^{\pi i r^2 \,z}\,dz.
> \end{aligned}
> $$
> We have
> $$
> \begin{aligned}c(r)=&\int\limits_{-1}^{i}\psi_T(z)\,e^{\pi i r^2 \,z}\,dz+\int\limits_{1}^{i}\psi_T(z)\,e^{\pi i r^2 \,z}\,dz
> -2\int\limits_{0}^{i}\psi_I(z)\,e^{\pi i r^2 \,z}\,dz\\
> &+2\int\limits_{i}^{i\infty}(\psi_T(z)-\psi_I(z))\,e^{\pi i r^2 \,z}\,dz.\nonumber
> \end{aligned}
> $$
> Next, we check that the functions $\psi_I,\psi_T$, and $\psi_S$ satisfy the following identity:
> $$\psi_T+\psi_S=\psi_I.$$
> Indeed, from definitions [[eq-psii-define]]-[[eq-psis-define]] we get
> $$
> \begin{aligned}\psi_T+\psi_S=&(h-h|_{-2}ST)|_{-2}T+(h-h|_{-2}ST)|_{-2}S\notag\\
> =&h|_{-2}T-h|_{-2}ST^2+h|_{-2}S-h|_{-2}STS.\notag\end{aligned}
> $$
> Note that $ST^2S$ belongs to $\Gamma_0(2)$. Thus, since $h\in M^!_{-2}\Gamma_0(2)$ we get
> $$\psi_T+\psi_S=h|_{-2}T-h|_{-2}STS. $$
> Now we observe that $T$ and $STS(ST)^{-1}$ are also in $\Gamma_0(2)$. Therefore,
> $$\psi_T+\psi_S=h|_{-2}T-h|_{-2}STS=h|_{-2}-h|ST=\psi_I.$$
> 
> Combining (eqn: c1) and (eqn: c2) we find
> $$
> \begin{aligned}c(r)=&\int\limits_{-1}^{i}\psi_T(z)\,e^{\pi i r^2 \,z}\,dz+\int\limits_{1}^{i}\psi_T(z)\,e^{\pi i r^2 \,z}\,dz
> -2\int\limits_{0}^{i}\psi_I(z)\,e^{\pi i r^2 \,z}\,dz\notag\\
> &-2\int\limits_{i}^{i\infty}\psi_S(z)\,e^{\pi i r^2 \,z}\,dz\notag\\
> =&b(r).\notag
> \end{aligned}
> $$
