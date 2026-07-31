---
id: b505f8a6a0f9
type: lemma
from: blueprint
lean:
  - SpherePacking.scale_finiteDensity
formalized: true
---

# Lemma — SpherePacking.scale_finiteDensity

## Statement

> [!lemma] SpherePacking.scale_finiteDensity
> Let $\mathcal{P}(X)$ be a [[spherepackingballs|sphere packing]] and $c$ a positive real number. Then, for all $R > 0$,
> 
> $$\Delta_{\mathcal{P}(cX)}(cR) = \Delta_{\mathcal{P}(X)}(R).$$

## Proof

> [!note]- Proof (click to expand)
> The proof follows by direct computation:
> 
> $$\Delta_{\mathcal{P}(cX)}(cR) = \frac{\operatorname{Vol}\!\left(\mathcal{P}(cX) \cap B_d(0, cR)\right)}{\operatorname{Vol}\!\left(B_d(0, cR)\right)} = \frac{c^d \cdot \operatorname{Vol}\!\left(\mathcal{P}(X) \cap B_d(0, R)\right)}{c^d \cdot \operatorname{Vol}\!\left(B_d(0, R)\right)}
> 
> = \Delta_{\mathcal{P}(X)}(R)$$
> 
> where the second equality follows from applying the fact that scaling a (measurable) set by a factor of $c$ scales its volume by a factor of $c^d$ to the fact that $\mathcal{P}(cX) \cap B_d(0, cR) = c \cdot (\mathcal{P}(X) \cap B_d(0, cR))$.

**Uses**: [[spherepackingfinitedensity]], [[spherepackingscale]].
