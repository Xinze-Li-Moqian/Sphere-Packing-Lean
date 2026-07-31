---
id: 687ba76775dc
type: definition
from: blueprint
lean:
  - D
formalized: true
---

# Definition — def:derivative

## Statement

> [!definition] def:derivative
> Let $F$ be a quasimodular form.
> We define the (normalized) derivative of $F$ as
> $$
> F' = DF := \frac{1}{2\pi i} \frac{\mathrm{d}}{\mathrm{d} z} F.
> $$

**Used by**: [[def-serre-der]], [[lemma-der-q-series]].

## Notes

> [!note]- Notes (click to expand)
> - The normalisation by $1/2\pi i$ makes $D$ act on $q$-expansions as $q\,\mathrm{d}/\mathrm{d}q$: it multiplies the $n$-th coefficient by $n$. That is why [[lemma-der-q-series]] and the coefficient estimates read as cleanly as they do.
> - $D$ does not preserve [[def-mk|modularity]] — it raises the weight by two and adds a term in $E_2$ ([[def-e2]]). The [[def-serre-der|Serre derivative]] is $D$ corrected by exactly that term, and is the derivative this development uses.
> - The hypothesis is a *quasimodular* form, which this pool does not define; see the debt row in [[notation]].
