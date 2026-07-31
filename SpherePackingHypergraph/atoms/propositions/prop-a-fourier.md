---
id: 1216fa6a3448
type: proposition
from: blueprint
lean:
  - MagicFunction.a.Fourier.eig_a
---

# Proposition — prop:a-fourier

## Statement

> [!proposition] prop:a-fourier
> $a(x)$ satisfies [[eq-a-fourier]].

## Proof

> [!note]- Proof (click to expand)
> We recall that the [[def-fourier-transform|Fourier transform]] of a Gaussian function is
> $$
> \mathcal{F}(e^{\pi i \|x\|^2 z})(y)=z^{-4}\,e^{\pi i \|y\|^2 \,(\frac{-1}{z}) }.
> $$
> Next, we exchange the contour integration with respect to $z$ variable and Fourier transform with respect to $x$ variable in (eqn:a-definition).
> This can be done, since the corresponding double integral converges absolutely. In this way we obtain
> $$
> \begin{aligned}
> \widehat{a}(y)=&\int\limits_{-1}^i\phi_0\Big(\frac{-1}{z+1}\Big)\,(z+1)^2\,z^{-4}\,e^{\pi i \|y\|^2 \,(\frac{-1}{z})}\,dz
> +\int\limits_{1}^i\phi_0\Big(\frac{-1}{z-1}\Big)\,(z-1)^2\,z^{-4}\,e^{\pi i \|y\|^2 \,(\frac{-1}{z})}\,dz\notag \\
> -&2\int\limits_{0}^i\phi_0\Big(\frac{-1}{z}\Big)\,z^2\,z^{-4}\,e^{\pi i \|y\|^2 \,(\frac{-1}{z})}\,dz +2\int\limits_{i}^{i\infty}\phi_0(z)\,z^{-4}\,e^{\pi i \|y\|^2 \,(\frac{-1}{z})}\,dz.\notag
> \end{aligned}
> $$
> Now we make a change of variables $w=\frac{-1}{z}$. We obtain
> $$
> \begin{aligned}
> \widehat{a}(y)=&\int\limits_{1}^i\phi_0\Big(1-\frac{1}{w-1}\Big)\,(\frac{-1}{w}+1)^2\,w^{2}\,e^{\pi i \|y\|^2 \,w}\,dw\notag\\
> +&\int\limits_{-1}^i\phi_0\Big(1-\frac{1}{w+1}\Big)\,(\frac{-1}{w}-1)^2\,w^2\,e^{\pi i \|y\|^2 \,w}\,dw\\
> -&2\int\limits_{i \infty}^i\phi_0(w)\,e^{\pi i \|y\|^2 \,w}\,dw +2\int\limits_{i}^{0}\phi_0\Big(\frac{-1}{w}\Big)\,w^{2}\,e^{\pi i \|y\|^2 \,w}\,dw.\notag
> \end{aligned}
> $$
> Since $\phi_0$ is $1$-[[periodicspherepacking|periodic]] we have
> $$
> \begin{aligned}
> \widehat{a}(y)\,=\,&\int\limits_{1}^i\phi_0\Big(\frac{-1}{z-1}\Big)\,(z-1)^2\,e^{\pi i \|y\|^2 \,z}\,dz
> +\int\limits_{-1}^i\phi_0\Big(\frac{-1}{z+1}\Big)\,(z+1)^2\,e^{\pi i \|y\|^2 \,z}\,dz\notag \\
> +&2\int\limits_{i}^{i\infty}\phi_0(z)\,e^{\pi i \|y\|^2 \,z}\,dz
> -2\int\limits_{0}^{i}\phi_0\Big(\frac{-1}{z}\Big)\,z^{2}\,e^{\pi i \|y\|^2 \,z}\,dz\notag \\
> \,=\,&a(y).
> \end{aligned}
> $$
> This finishes the proof of the proposition.

**Uses**: [[def-a-definition]], [[def-e2]], [[lemma-ek-fourier]], [[lemma-gaussian-fourier]], [[prop-a-schwartz]].
