---
id: 037ed214719d
type: proposition
---

# Proposition — prop:a-double-zeros

## Statement

> [!proposition] prop:a-double-zeros
> For $r>\sqrt{2}$ we can express $a(r)$ in the following form
> $$
> a(r)=-4\sin(\pi r^2/2)^2\,\int\limits_{0}^{i\infty}\phi_0\Big(\frac{-1}{z}\Big)\,z^2\,e^{\pi i r^2 \,z}\,dz.
> $$

## Proof

> [!note]- Proof (click to expand)
> We denote the right hand side of [[eq-a-double-zeroes]] by $d(r)$.
> Convergence of the integral for $r > \sqrt{2}$ follows from Corollary~[[cor-phi0-near-0-infty]].
> We can write 
> $$
> \begin{aligned}
> d(r)=&\int\limits_{-1}^{i\infty-1}\phi_0\Big(\frac{-1}{z+1}\Big)\,(z+1)^2\,e^{\pi i r^2 \,z}\,dz-
> 2\int\limits_{0}^{i\infty}\phi_0\Big(\frac{-1}{z}\Big)\,z^2\,e^{\pi i r^2 \,z}\,dz\notag\\
> +&\int\limits_{1}^{i\infty+1}\phi_0\Big(\frac{-1}{z-1}\Big)\,(z-1)^2\,e^{\pi i r^2 \,z}\,dz.\notag
> \end{aligned}
> $$
> From [[eq-phi0-trans-s]] we deduce that if $r>\sqrt{2}$ then
> $\phi_0\Big(\frac{-1}{z}\Big)\,z^2\,e^{\pi i r^2 \,z}\to 0$ as $\Im(z)\to\infty$. Therefore, we can deform the paths of integration
> and rewrite
> $$
> \begin{aligned}
> d(r)=&\int\limits_{-1}^{i}\phi_0\Big(\frac{-1}{z+1}\Big)\,(z+1)^2\,e^{\pi i r^2 \,z}\,dz
> +\int\limits_{i}^{i\infty}\phi_0\Big(\frac{-1}{z+1}\Big)\,(z+1)^2\,e^{\pi i r^2 \,z}\,dz\notag\\
> -2&\int\limits_{0}^{i}\phi_0\Big(\frac{-1}{z}\Big)\,z^2\,e^{\pi i r^2 \,z}\,dz
> -2\int\limits_{i}^{i\infty}\phi_0\Big(\frac{-1}{z}\Big)\,z^2\,e^{\pi i r^2 \,z}\,dz\notag\\
> +&\int\limits_{1}^{i}\phi_0\Big(\frac{-1}{z-1}\Big)\,(z-1)^2\,e^{\pi i r^2 \,z}\,dz
> +\int\limits_{i}^{i\infty}\phi_0\Big(\frac{-1}{z-1}\Big)\,(z-1)^2\,e^{\pi i r^2 \,z}\,dz.\notag
> \end{aligned}
> $$
> Now from [[eq-phi0-trans-s]] we find
> $$
> \begin{aligned}&\phi_0\Big(\frac{-1}{z+1}\Big)\,(z+1)^2-2\phi_0\Big(\frac{-1}{z}\Big)\,z^2+
> \phi_0\Big(\frac{-1}{z-1}\Big)\,(z-1)^2=\notag\\
> &\phi_0(z+1)\,(z+1)^2-2\phi_0(z)\,z^2+\phi_0(z-1)\,(z-1)^2\notag\\
> &-\frac{12i}{\pi}\,\Big(\phi_{-2}(z+1)\,(z+1)-2\phi_{-2}(z)\,z+\phi_{-2}(z-1)\,(z-1)\Big)\notag\\
> &-\frac{36}{\pi^2}\Big(\phi_{-4}(z+1)-2\phi_{-4}(z)+\phi_{-4}(z-1)\Big)=\notag\\
> &2\phi_0(z).
> \end{aligned}
> $$
> Thus, we obtain
> $$
> \begin{aligned}
> d(r)=&\int\limits_{-1}^{i}\phi_0\Big(\frac{-1}{z+1}\Big)\,(z+1)^2\,e^{\pi i r^2 \,z}\,dz
> -2\int\limits_{0}^{i}\phi_0\Big(\frac{-1}{z}\Big)\,z^2\,e^{\pi i r^2 \,z}\,dz\notag\\
> +&\int\limits_{1}^{i}\phi_0\Big(\frac{-1}{z-1}\Big)\,(z-1)^2\,e^{\pi i r^2 \,z}\,dz
> +2\int\limits_{i}^{i\infty}\phi_0(z)\,e^{\pi i r^2 \,z}\,dz=a(r).\notag
> \end{aligned}
> $$
> This finishes the proof.
