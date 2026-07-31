---
id: 99e5b65246c6
type: theorem
lean:
  - ramanujan_E₂
  - ramanujan_E₄
  - ramanujan_E₆
  - ramanujan_E₂'
  - ramanujan_E₄'
  - ramanujan_E₆'
formalized: true
---

# Theorem — thm:ramanujan-formula

## Statement

> [!theorem] thm:ramanujan-formula
> We have
> $$
> \begin{aligned}
> E_2' &= \frac{E_2^2 - E_4}{12}  \\
> E_4' &= \frac{E_2 E_4 - E_6}{3}  \\
> E_6' &= \frac{E_2 E_6 - E_4^2}{2} 
> \end{aligned}
> $$

## Proof

> [!note]- Proof (click to expand)
> In terms of Serre derivatives, these are equivalent to
> $$
> \begin{aligned}
> \partial_{1}E_2 &= -\frac{1}{12} E_4  \\
> \partial_{4}E_4 &= -\frac{1}{3} E_6  \\
> \partial_{6}E_6 &= -\frac{1}{2} E_4^2 
> \end{aligned}
> $$
> By Theorem [[thm-serre-der-modularity]], all the Serre derivatives are, in fact, modular.
> To be precise, the modularity of $\partial_{4} E_4$ and $\partial_6 E_6$ directly follows from Theorem [[thm-serre-der-modularity]], and that of $\partial_{1}E_2$ follows from [[eq-e2-transform-general]].
> Differentiating and squaring then gives us the following:
> $$
> \begin{aligned}
> E_2'|_{4}\gamma &= E_2' - \frac{ic}{\pi(cz + d)} E_2 - \frac{3c^2}{\pi^2 (cz + d)^2}  \\
> E_2^2|_{4}\gamma &= E_2^2 - \frac{12ic}{\pi(cz + d)} E_2 - \frac{36c^2}{\pi^2 (cz + d)^2} 
> \end{aligned}
> $$
> Hence, [[eq-de2]]$-\frac{1}{12}$(eqn:E2sq-transform) is a modular form of weight 4.
> By [[cor-dim-mf]], they should be multiples of $E_4, E_6, E_4^2$, and the proportionality constants can be determined by observing the constant terms of $q$-expansions.
