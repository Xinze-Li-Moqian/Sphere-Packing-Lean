---
id: 7553544e1244
type: theorem
---

# Theorem — thm:g1

## Statement

> [!theorem] thm:g1
> The function
> $$g(x):=\frac{\pi\,i}{8640}a(x)+\frac{i}{240\pi}\,b(x)$$
> satisfies conditions [[eq-g1]]--[[eq-g3]].

## Proof

> [!note]- Proof (click to expand)
> First, we prove that [[eq-g1]] holds. By Propositions~[[prop-a-double-zeros]] and [[prop-b-double-zeros]] we know that for $r>\sqrt{2}$
> $$ g(r)=\frac{\pi}{2160}\,\sin(\pi r^2/2)^2\,\int\limits_0^\infty A(t)\,e^{-\pi r^2 t}\,dt$$
> where $$A(t)=-t^2\phi_0(i/t)-\frac{36}{\pi^2}\,\psi_I(it).$$
> from the Proposition~[[prop-ineqa]] we know that $A(t)<0\quad\mbox{for}\;t\in(0,\infty).$
> Therefore identity (eqn:g A) implies [[eq-g1]].
> 
> Next, we prove [[eq-g2]]. By Propositions~[[prop-a-another-integral]] and~[[prop-b-another-integral]] we know that for $r>0$
> $$ \widehat{g}(r)=\frac{\pi}{2160}\,\sin(\pi r^2/2)^2\,\int\limits_0^\infty B(t)\,e^{-\pi r^2 t}\,dt$$
> where $$B(t)=-t^2\phi_0(i/t)+\frac{36}{\pi^2}\,\psi_I(it).$$
> 
> Finally, the property [[eq-g3]] readily follows from Proposition~[[prop-a0]] and Proposition~[[prop-b0]]. This finishes the proof of Theorems~[[thm-g1]] and~[[thm-g]].
