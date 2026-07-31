---
id: e68da0249073
type: proposition
lean:
  - MagicFunction.a.SpecialValues.a_zero
formalized: true
---

# Proposition — prop:a0

## Statement

> [!proposition] prop:a0
> We have $a(0) = -\frac{8640\,i}{\pi}$.

**Used by**: [[thm-g1]].

## Proof

> [!note]- Proof (click to expand)
> Let $r\to0^+$ in [[prop-a-another-integral]]. Every factor there carries $\sin^2(\pi r^2/2)\sim\frac{\pi^2r^4}{4}$, so only the term with a matching $r^{-4}$ pole survives the limit:
> $$a(0)=\lim_{r\to0}4i\,\sin^2\!\big(\tfrac{\pi r^2}{2}\big)\cdot\Big(-\frac{8640}{\pi^3r^4}\Big)=4i\cdot\frac{\pi^2}{4}\cdot\Big(-\frac{8640}{\pi^3}\Big)=-\frac{8640\,i}{\pi}.$$
> The remaining terms — $\frac{36}{\pi^3(r^2-2)}$, $\frac{18144}{\pi^3 r^2}$ and the absolutely convergent integral — are $O(r^{-2})$ or bounded, and vanish against $r^4$.
>
> *(As imported the value read $-\frac{i}{8640}$. That is inconsistent twice over: with the limit above, and with [[eq-g3]] — the normalization of [[thm-g1]] gives $g(0)=\frac{\pi i}{8640}\,a(0)$, which equals $1$ exactly for $a(0)=-\frac{8640\,i}{\pi}$. Corrected.)*

**Uses**: [[prop-a-another-integral]].
