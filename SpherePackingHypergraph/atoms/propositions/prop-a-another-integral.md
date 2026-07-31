---
id: 3c867e76a86b
type: proposition
---

# Proposition — prop:a-another-integral

## Statement

> [!proposition] prop:a-another-integral
> For $r\geq0$ we have
> $$
> \begin{aligned}a(r)=&4i\,\sin(\pi r^2/2)^2\,\Bigg(\frac{36}{\pi^3\,(r^2-2)}-\frac{8640}{\pi^3\,r^4}+\frac{18144}{\pi^3\,r^2}\\ +&\int\limits_0^\infty\,\left(t^2\,\phi_0\Big(\frac{i}{t}\Big)-\frac{36}{\pi^2}\,e^{2\pi t}+\frac{8640}{\pi}\,t-\frac{18144}{\pi^2}\right)\,e^{-\pi r^2 t}\,dt \Bigg) .\notag\end{aligned}
> $$
> The integral converges absolutely for all $r\in\mathbb{R}_{\geq 0}$.

## Proof

> [!note]- Proof (click to expand)
> Suppose that $r>\sqrt{2}$. Then by Proposition [[prop-a-double-zeros]]
> $$a(r)=4i\,\sin(\pi r^2/2)^2\,\int\limits_{0}^{\infty}\phi_0(i/t)\,t^2\,e^{-\pi r^2 t}\,dt. $$
> From [[eq-phi0-trans-s]] we obtain
> $$
> \phi_0(i/t)\,t^2=\frac{36}{\pi^2}\,e^{2 \pi t}-\frac{8640}{\pi}\,t+\frac{18144}{\pi^2}+O(t^2\,e^{-2\pi t})\quad\mbox{as}\;t\to\infty.
> $$
> For $r>\sqrt{2}$ we have
> $$
> \int\limits_0^\infty \left(\frac{36}{\pi^2}\,e^{2 \pi t}+\frac{8640}{\pi}\,t+\frac{18144}{\pi^2}\right)\,e^{-\pi r^2 t}\,dt
> =\frac{36}{\pi^3\,(r^2-2)}-\frac{8640}{\pi^3\,r^4}+\frac{18144}{\pi^3\,r^2}.$$
> Therefore, the identity [[eq-a-another-integral]] holds for $r>\sqrt{2}$.
> 
> On the other hand, from the definition (eqn:a-definition) we see that $a(r)$ is analytic in some neighborhood of $[0,\infty)$. The asymptotic expansion (eqn: phi asymptotic) implies that the right hand side of [[eq-a-another-integral]] is also analytic in some neighborhood of $[0,\infty)$. Hence, the identity [[eq-a-another-integral]] holds on the whole interval $[0,\infty)$. This finishes the proof of the proposition.
