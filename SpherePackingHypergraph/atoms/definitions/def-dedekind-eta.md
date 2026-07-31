---
id: bd0bac6e3f1e
type: definition
from: blueprint
lean:
  - ModularForm.eta
formalized: true
---

# Definition — def:dedekind_eta

## Statement

> [!definition] def:dedekind_eta
> The Dedekind eta function is defined as
> $$
> \eta(z) = q^{1/24} \prod_{n \ge 1} (1 - q^n)
> $$
> where $q = e^{2\pi i z}$.

**Used by**: [[def-disc-definition]], [[lemma-dedekind-eta-transformation]].

## Notes

> [!note]- Notes (click to expand)
> - Weight $1/2$, so it is not itself in any [[def-mk|$M_k$]] — but its powers are: $\eta^{24} = $ [[def-disc-definition|$\Delta$]], the first [[def-cusp-form|cusp form]] of level one.
> - The product form makes its non-vanishing on the upper half-plane immediate, which is what allows division by it; the [[def-th00-th01-th10|theta functions]] are quotients of eta at scaled arguments, and that is how their transformation behaviour is obtained.
