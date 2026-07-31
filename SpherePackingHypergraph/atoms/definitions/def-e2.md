---
id: 0e7b52d79860
type: definition
from: blueprint
lean:
  - E₂_eq
formalized: true
---

# Definition — def:E2

## Statement

> [!definition] def:E2
> We set
> $$
> E_2(z):= 1-24\sum_{n=1}^\infty \sigma_1(n)\,e^{2\pi i n z}.
> $$

**Used by**: [[cor-logder-disc-e2]], [[cor-mlde-pos]], [[def-fg-definition]], [[def-phi4-phi2-phi0]].

## Notes

> [!note]- Notes (click to expand)
> - Formally the $k=2$ case of the [[def-ek|Eisenstein series]], but the defining sum is not absolutely convergent there, and the function one gets is not modular: it picks up an extra term under $S$ ([[def-gamma-generators]]). It is [[def-derivative|quasimodular]] instead.
> - That failure is exactly measured, which is what makes it usable: subtracting the right multiple of $E_2$ turns the [[def-derivative|derivative]] — which does not preserve modularity — into the [[def-serre-der|Serre derivative]], which does.
> - It appears throughout the $-1$ eigenfunction construction for that reason, in $F$ and $G$ ([[def-fg-definition]]) and in $H_2, H_3, H_4$ ([[def-h2-h3-h4]]).
