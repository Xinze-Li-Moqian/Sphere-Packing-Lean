---
id: 6c4eda959813
type: proposition
---

# Proposition — prop:ineqB

## Statement

> [!proposition] prop:ineqB
> Consider the function $B:(0,\infty)\to\mathbb{C}$ defined as
> $$
> B(t) := -t^2\phi_0(i/t)+\frac{36}{\pi^2}\,\psi_I(it)
> $$
> Then
> $$
> B(t) > 0
> $$
> for all $t > 0$.

## Proof

> [!note]- Proof (click to expand)
> By [[lemma-ineqabnew-equiv]], the inequality $B(t)>0$ ([[eq-ineqb]]) is equivalent to $F(it)-\frac{18}{\pi^2}G(it)>0$ ([[eq-ineqbnew]]).
>
> That is [[cor-ineqbnew]], and it is the delicate half: unlike the sum, the difference requires knowing that the ratio $Q(t)=F(it)/G(it)$ stays *below* its limit $\frac{18}{\pi^2}$ at $t\to0^+$ — monotonicity of $Q$ ([[prop-qdec]], via [[lemma-qlim]]) is exactly what closes it, together with the positivity of $G$ from [[lemma-f-g-pos]].
>
> As with [[prop-ineqa]]: numerically verified in [[ref-via2017]] §7, replaced by the algebraic argument of [[ref-lee]] in the form assembled here.

**Uses**: [[cor-ineqbnew]], [[lemma-f-g-phi-psi-identities]], [[lemma-ineqabnew-equiv]].
