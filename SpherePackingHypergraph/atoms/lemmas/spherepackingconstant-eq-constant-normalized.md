---
id: f7dfadfc1c2b
type: lemma
from: blueprint
lean:
  - SpherePacking.constant_eq_constant_normalized
formalized: true
---

# Lemma — SpherePacking.constant_eq_constant_normalized

## Statement

> [!lemma] SpherePacking.constant_eq_constant_normalized
> $$\Delta_d = \sup\limits_{\substack{\mathcal{P} \subset \mathbb{R}^d \\ \text{sphere packing} \\ \text{sep.~rad.} = 1}} \Delta_{\mathcal{P}}$$

**In terms of**: [[spherepackingconstant]], [[def-disc-definition]].

## Proof

> [!note]- Proof (click to expand)
> That the supremum over packings of unit [[spherepackingdensity|density]] is at most the [[spherepackingconstant|sphere packing constant]] is obvious. For the reverse inequality, let $\mathcal{P}(X)$ be any [[spherepackingballs|sphere packing]] with [[spherepackingballs|separation radius]] $r$. We know, from Lemma [[spherepackingscale-density]], that the density of $\mathcal{P}(X)$ is equal to that of the [[spherepackingscale|scaled packing]] $\mathcal{P}\!\left(\frac{X}{r}\right)$. Since the scaled packing has separation radius $1$, its density is naturally at most the supremum over all packings of unit density, meaning that the same is true of $\mathcal{P}(X)$.

**Uses**: [[spherepackingconstant]], [[spherepackingdensity]].
