---
id: 5545407ca679
type: proposition
from: blueprint
lean:
  - MagicFunction.b.Fourier.eig_b
formalized: true
---

# Proposition — prop:b-fourier

## Statement

> [!proposition] prop:b-fourier
> $b(x)$ satisfies [[eq-b-fourier]].

## Proof

> [!note]- Proof (click to expand)
> Here, we repeat the arguments used in the proof of Proposition [[prop-a-fourier]].
> We use identity [[eq-gaussian-fourier]] and change contour integration in $z$ and [[def-fourier-transform|Fourier transform]] in $x$. Thus we obtain
> $$
> \begin{aligned}
> \mathcal{F}(b)(x)= & \int\limits_{-1}^{i}\psi_T(z)\,z^{-4}\,e^{\pi i \|x\|^2 (\frac{-1}{z})}\,dz
> + \int\limits_{1}^{i}\psi_T(z)\,z^{-4}\,e^{\pi i \|x\|^2 (\frac{-1}{z})}\,dz \notag \\
> -& 2\,\int\limits_{0}^{i}\psi_I(z)\,z^{-4}\,e^{\pi i \|x\|^2 (\frac{-1}{z})}\,dz
> - 2\,\int\limits_{i}^{i\infty}\psi_S(z)\,z^{-4}\,e^{\pi i \|x\|^2 (\frac{-1}{z})}\,dz. \notag
> \end{aligned}
> $$
> We make the change of variables $w=\frac{-1}{z}$ and arrive at
> $$
> \begin{aligned}
> \mathcal{F}(b)(x)= & \int\limits_{1}^{i}\psi_T\Big(\frac{-1}{w}\Big)\,w^{2}\,e^{\pi i \|x\|^2 w}\,dw
> + \int\limits_{-1}^{i}\psi_T\Big(\frac{-1}{w}\Big)\,w^{2}\,e^{\pi i \|x\|^2 w}\,dw \notag \\
> -& 2\,\int\limits_{i\infty}^{i}\psi_I\Big(\frac{-1}{w}\Big)\,w^{2}\,e^{\pi i \|x\|^2 w}\,dw
> - 2\,\int\limits_{i}^{0}\psi_S\Big(\frac{-1}{w}\Big)\,w^{2}\,e^{\pi i \|x\|^2 w}\,dw.\notag
> \end{aligned}
> $$
> Now we observe that the definitions [[eq-psii-define]]--[[eq-psis-define]] imply
> $$
> \begin{aligned}
> \psi_T|_{-2}S=&-\psi_T \notag \\
> \psi_I|_{-2}S=&\psi_S \notag \\
> \psi_S|_{-2}S=&\psi_I. \notag
> \end{aligned}
> $$
> Therefore, we arrive at
> $$
> \begin{aligned}
> \mathcal{F}(b)(x)= & \int\limits_{1}^{i}-\psi_T(z)\,e^{\pi i \|x\|^2 z}\,dz
> + \int\limits_{-1}^{i}-\psi_T(z)\,e^{\pi i \|x\|^2 z}\,dz \notag \\
> +& 2\,\int\limits_{i}^{i\infty}\psi_S(z)\,e^{\pi i \|x\|^2 z}\,dz
> + 2\,\int\limits_{0}^{i}\psi_I(z)\,e^{\pi i \|x\|^2 w}\,dw.\notag
> \end{aligned}
> $$
> Now from [[eq-b-definition]] we see that
> $$ \mathcal{F}(b)(x)=-b(x). $$

**Uses**: [[def-b-definition]], [[def-psii-psit-psis]], [[lemma-gaussian-fourier]], [[prop-b-schwartz]].
