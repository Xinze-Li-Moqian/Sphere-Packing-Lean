---
id: 72416c476cbb
type: lemma
---

# Lemma — lemma:bound-J2-J4-J6

## Statement

> [!lemma] lemma:bound-J2-J4-J6
> There exist $C_1, C_2 > 0$ such that
> $$
> \begin{aligned}
> |J_2(r)|, |J_4(r)| &\le C_1 e^{-\pi r} \\
> |J_6(r)| &\le C_2 \frac{e^{\pi (r + 1)}}{r + 1}
> \end{aligned}
> $$

**In terms of**: [[def-b-definition]].

## Proof

> [!note]- Proof (click to expand)
> **$J_2$ and $J_4$.** By [[def-b-definition]] these run along the horizontal segments from $\pm1+i$ to $i$: there $z=x+i$, so $\Im z=1$, and [[lemma-psi-bound]] gives the uniform bound $|\psi_T(z)|\le C_Te^{2\pi}$. Since $|e^{\pi irz}|=e^{-\pi r\,\Im z}=e^{-\pi r}$ and each contour has length $1$,
> $$|J_2(r)|,\;|J_4(r)|\;\le\;C_Te^{2\pi}\,e^{-\pi r}\;=:\;C_1e^{-\pi r}.$$
>
> **$J_6$.** Here $z=it$, $t\in[1,\infty)$, and the integrand is $\psi_S$, the one $\psi$ that *decays* upward: $|\psi_S(it)|\le C_Se^{-\pi t}$ by [[lemma-psi-bound]]. So for $r\ge0$
> $$|J_6(r)|\;\le\;2C_S\int_1^\infty e^{-\pi t}e^{-\pi rt}\,dt\;=\;\frac{2C_S}{\pi}\,\frac{e^{-\pi(r+1)}}{r+1},$$
> which implies the stated bound a fortiori. (The sharp form has the *decaying* exponential $e^{-\pi(r+1)}$; the exponent as imported reads $e^{\pi(r+1)}$, which is true but far weaker — the decay is what [[prop-b-schwartz]] actually consumes.)
>
> Together with [[lemma-bound-j1-j3-j5]] this controls all six pieces of $b_{\mathrm{rad}}$, uniformly on $r\ge0$.
