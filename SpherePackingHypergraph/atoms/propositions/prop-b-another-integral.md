---
id: 1761cd3e5780
type: proposition
---

# Proposition — prop:b-another-integral

## Statement

> [!proposition] prop:b-another-integral
> For $r\geq0$ we have
> $$b(r)=4i\,\sin(\pi r^2/2)^2\,\left(\frac{144}{\pi\,r^2}+\frac{1}{\pi\,(r^2-2)}+\int\limits_0^\infty\,\left(\psi_I(it)-144-e^{2\pi t}\right)\,e^{-\pi r^2 t}\,dt\right).$$
> The integral converges absolutely for all $r\in\mathbb{R}_{\geq 0}$.

## Proof

> [!note]- Proof (click to expand)
> The proof is analogous to the proof of Proposition [[prop-a-another-integral]].
> First, suppose that $r>\sqrt{2}$. Then by Proposition [[prop-b-double-zeros]]
> $$b(r)=4i\,\sin(\pi r^2/2)^2\,\int\limits_{0}^{\infty}\psi_I(it)\,e^{-\pi r^2 t}\,dt. $$
> From [[eq-psi-fourier-i]] we obtain
> $$
> \psi_I(it)=e^{2\pi t}+144+O(e^{-\pi t})\quad\mbox{as}\;t\to\infty.
> $$
> For $r>\sqrt{2}$ we have
> $$
> \int\limits_0^\infty \left(e^{2\pi t}+144\right)\,e^{-\pi r^2 t}\,dt
> =\frac{1}{\pi\,(r^2-2)}+\frac{144}{\pi\,r^2}.$$
> Therefore, the identity [[eq-b-another-integral]] holds for $r>\sqrt{2}$.
> 
> On the other hand, from the definition [[eq-b-definition]] we see that $b(r)$ is analytic in some neighborhood of $[0,\infty)$. The asymptotic expansion (eqn: psi asymptotic) implies that the right hand side of [[eq-b-another-integral]] is also analytic in some neighborhood of $[0,\infty)$. Hence, the identity [[eq-b-another-integral]] holds on the whole interval $[0,\infty)$. This finishes the proof of the proposition.
