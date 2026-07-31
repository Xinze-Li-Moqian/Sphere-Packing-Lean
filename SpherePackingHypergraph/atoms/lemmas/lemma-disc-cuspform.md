---
id: 9cb13326fb7b
type: lemma
lean:
  - CuspForm.discriminant
formalized: true
---

# Lemma — lemma:disc-cuspform

## Statement

> [!lemma] lemma:disc-cuspform
> $\Delta(z) \in M_{12}(\Gamma_1)$.
> Especially, we have
> $$
> \Delta\left(-\frac{1}{z}\right) = z^{12} \Delta(z).
> $$
> Also, it vanishes at the unique cusp, i.e. it is a cusp form of level $\Gamma_1$ and weight $12$.

## Proof

> [!note]- Proof (click to expand)
> The fact that it is invariant under translation is clear from the definition, so we only need to check transformation under $S$. Now, note that $\eta^{24} = \Delta$, and from [[lemma-dedekind-eta-transformation]] we have $\eta(-1/z) = \sqrt{-iz} \eta(z)$, so $\Delta(-1/z) = z^{12} \Delta(z)$ as required.
