---
id: f77a3ff132bb
type: lemma
from: blueprint
lean:
  - SpherePacking.scale_density
formalized: true
---

# Lemma — SpherePacking.scale_density

## Statement

> [!lemma] SpherePacking.scale_density
> Let $\mathcal{P}(X)$ be a [[spherepackingballs|sphere packing]] and $c$ a positive real number. Then, the [[spherepackingdensity|density]] of the [[spherepackingscale|scaled packing]] $\mathcal{P}(cX)$ is equal to the density of the original packing $\mathcal{P}(X)$.

## Proof

> [!note]- Proof (click to expand)
> One can show, using relatively unsophisticated real analysis, that
> 
> $$\limsup_{R \to \infty} \Delta_{\mathcal{P}(cX)}(R) = \limsup_{cR \to \infty} \Delta_{\mathcal{P}(cX)}(cR)$$
> 
> Lemma [[spherepackingscale-finitedensity]] tells us that $\Delta_{\mathcal{P}(cX)}(cR) = \Delta_{\mathcal{P}(X)}(R)$ for every $R > 0$. Therefore,
> 
> $$\limsup_{cR \to \infty} \Delta_{\mathcal{P}(cX)}(cR) = \limsup_{cR \to \infty} \Delta_{\mathcal{P}(X)}(R) = \limsup_{R \to \infty} \Delta_{\mathcal{P}(X)}(R)$$
> 
> where the second equality is the result of a similar change of variables to the one done above.

**Uses**: [[spherepackingscale]].
