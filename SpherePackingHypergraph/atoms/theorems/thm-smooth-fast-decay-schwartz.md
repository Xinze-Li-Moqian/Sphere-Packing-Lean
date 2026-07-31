---
id: b02d1c9c4844
type: theorem
---

# Theorem — thm:smooth-fast-decay-schwartz

## Statement

> [!theorem] thm:smooth-fast-decay-schwartz
> Assume $f : \mathbb{R} \to \mathbb{C}$ is smooth on $[0, \infty)$ and for all $k, n \in \mathbb{N}$, there exists $C \in \mathbb{R}$ such that
> $$
> x^{\frac{k}{2}} \cdot |f^{(n)}(x)| \leq C.
> $$
> Then, for all $d \in \mathbb{N}$, the function
> $$
> f_d : \mathbb{R}^d \to \mathbb{C}, \quad f_d(x) := f(\|x\|^2)
> $$
> is a [[def-schwartz-space|Schwartz function]].

## Proof

> [!note]- Proof (click to expand)
> Two things to prove about $f_d(x)=f(\|x\|^2)$: smoothness, and decay of every derivative faster than every inverse power ([[def-schwartz-space|the Schwartz conditions]]).
>
> **Smoothness.** $\|x\|^2$ is a polynomial, and $f$ is smooth on $[0,\infty)$; a smooth function on the half-line extends to a smooth function on $\mathbb{R}$ (Whitney/Seeley extension), so $f_d$ is a composition of smooth maps.
>
> **Structure of the derivatives.** By induction on $|\alpha|$: every partial derivative has the form
> $$\partial^\alpha f_d(x)\;=\;\sum_{m\le|\alpha|}\;\sum_{|\beta|\le|\alpha|}c_{\alpha,\beta,m}\,x^\beta\,f^{(m)}(\|x\|^2),$$
> with finitely many constants $c$. Indeed differentiating one term by $x_j$ either lowers $x^\beta$ (keeping $m$) or raises $m$ by one and multiplies by $2x_j$ — both of the allowed shapes.
>
> **Decay.** Fix $\alpha$ and a target power $N$. For each term above, apply the hypothesis with $n=m$ and $k=2(N+|\beta|)$: writing $t=\|x\|^2$,
> $$\big|x^\beta f^{(m)}(t)\big|\;\le\;\|x\|^{|\beta|}\cdot C\,t^{-k/2}\;=\;C\,\|x\|^{|\beta|-k}\;=\;C\,\|x\|^{-2N-|\beta|}\;\le\;C\,\|x\|^{-N}$$
> for $\|x\|\ge1$; on $\|x\|\le1$ everything is bounded by continuity. So $\sup_x\|x\|^N|\partial^\alpha f_d(x)|<\infty$ for every $\alpha$ and $N$, which is exactly the Schwartz condition.
>
> This is the criterion through which [[prop-a-schwartz]] and [[prop-b-schwartz]] pass from one-variable estimates on $a_{\mathrm{rad}}, b_{\mathrm{rad}}$ to the eight-dimensional statement.
