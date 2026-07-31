---
id: a4601ae2a7a9
type: theorem
lean:
  - E8Packing_density
formalized: true
---

# Theorem — E8Packing-density

## Statement

> [!theorem] E8Packing-density
> We have $\Delta_{\mathcal{P}(E_8)} = \frac{\pi^4}{384}$.

## Proof

> [!note]- Proof (click to expand)
> By [[theorem-psp-density]], we have $\Delta_{\mathcal{P}(E_8)} = |E_8 / E_8| \cdot \frac{\operatorname{Vol}\!\left(\mathcal{B}_8(\sqrt{2} / 2)\right)}{\mathrm{Covol}(E_8)} = \frac{\pi^4}{384}$, where the last equality follows from [[e8packing-covol]] and the formula for volume of a ball: $\operatorname{Vol}\!\left(\mathcal{B}_d(R)\right) = R^d \pi^{d / 2} / \Gamma\left(\frac{d}{2} + 1\right)$.
