---
id: 3cc38c337f88
type: lemma
from: blueprint
lean:
  - SpherePacking.finiteDensity_le
  - SpherePacking.finiteDensity_ge
formalized: true
---

# Lemma — lemma:sp-finite-density-bound

## Statement

> [!lemma] lemma:sp-finite-density-bound
> For any $R > 0$,
> 
> $$\left|X \cap \mathcal{B}_d\left(R - \frac{r}{2}\right)\right| \cdot \frac{\mathrm{Vol}\left(\mathcal{B}_d\left(\frac{r}{2}\right)\right)}{\mathrm{Vol}(\mathcal{B}_d(R))}
> \leq \Delta_{\mathcal{P}}(R)
> \leq \left|X \cap \mathcal{B}_d\left(R + \frac{r}{2}\right)\right| \cdot \frac{\mathrm{Vol}\left(\mathcal{B}_d\left(\frac{r}{2}\right)\right)}{\mathrm{Vol}(\mathcal{B}_d(R))}$$

**In terms of**: [[def-disc-definition]].

## Proof

> [!note]- Proof (click to expand)
> The high level idea is to prove that $\mathcal{P} \cap \mathcal{B}_d(R) = \left(\bigcup_{x \in X} \mathcal{B}_d\left(x, \frac{r}{2}\right)\right) \subseteq \bigcup_{x \in X \cap \mathcal{B}_d\left(R + \frac{r}{2}\right)} \mathcal{B}_d\left(x, \frac{r}{2}\right)$, and a similar inequality for the upper bound. The rest follows by rearranging and using the fact that the balls are pairwise disjoint.

**Uses**: [[spherepackingfinitedensity]].
