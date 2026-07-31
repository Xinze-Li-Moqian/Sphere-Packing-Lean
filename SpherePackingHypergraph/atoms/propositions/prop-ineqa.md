---
id: bac2f60bbd19
type: proposition
---

# Proposition — prop:ineqA

## Statement

> [!proposition] prop:ineqA
> Consider the function $A:(0,\infty)\to\mathbb{C}$ defined as
> $$
> A(t):=-t^2\phi_0(i/t)-\frac{36}{\pi^2}\,\psi_I(it).
> $$
> Then
> $$
> A(t) < 0
> $$
> for all $t > 0$.

## Proof

> [!note]- Proof (click to expand)
> By [[lemma-ineqabnew-equiv]], the inequality $A(t)<0$ ([[eq-ineqa]]) is equivalent to $F(it)+\frac{18}{\pi^2}G(it)>0$ ([[eq-ineqanew]]) — the change of variables trades the transcendental combination of [[def-phi4-phi2-phi0|$\phi_0$]] and [[def-psii-psit-psis|$\psi_I$]] for the two (quasi)modular forms [[def-fg-definition|$F$ and $G$]].
>
> And [[eq-ineqanew]] holds by [[cor-ineqanew]]: both $F(it)$ and $G(it)$ are strictly positive on $t>0$ ([[lemma-f-g-pos]]), being — by Ramanujan&#8217;s identity — squares and products of $q$-series with positive coefficients, so the sum is positive term by term.
>
> This route is the point of the whole $F,G$ apparatus: [[ref-via2017]] established these sign conditions by interval arithmetic (§7), and the chain assembled here — following [[ref-lee]] — replaces the numerics with a positivity argument one can read.

**Uses**: [[cor-ineqanew]], [[lemma-f-g-phi-psi-identities]], [[lemma-f-g-pos]], [[lemma-ineqabnew-equiv]].
