---
id: 7ad9d222d25f
type: theorem
lean:
  - PeriodicSpherePacking.density_eq
formalized: true
---

# Theorem — theorem:psp-density

## Statement

> [!theorem] theorem:psp-density
> For a periodic [[spherepackingballs|sphere packing]] $\mathcal{P} = \mathcal{P}(X)$ with centers $X$ periodic to the [[iszlattice|lattice]] $\Lambda$ and separation $r$,
> 
> $$\Delta_{\mathcal{P}} = |X / \Lambda| \cdot \frac{\operatorname{Vol}\!\left(\mathcal{B}_d(r / 2)\right)}{\operatorname{Vol}\!\left(\mathbb{R}^d / \Lambda\right)}$$

## Proof

> [!note]- Proof (click to expand)
> Fix any fundamental domain $\mathcal{D}$ (induced by any basis) of the lattice $\Lambda$. Combining [[lemma-sp-finite-density-bound]], [[lemma-lattice-points-bound]] and [[lemma-periodic-points-bounds]], we get the following inequality for the *finite* [[spherepackingdensity|density]]:
> 
> $$|X / \Lambda| \cdot \frac{\operatorname{Vol}\!\left(\mathcal{B}_d(r / 2)\right)}{\operatorname{Vol}\!\left(\mathbb{R}^d / \Lambda\right)} \cdot \frac{\operatorname{Vol}\!\left(\mathcal{B}_d(R - r / 2 - 2L)\right)}{\operatorname{Vol}\!\left(\mathcal{B}_d(R)\right)}
> \leq \Delta_{\mathcal{P}}(R)
> \leq |X / \Lambda| \cdot \frac{\operatorname{Vol}\!\left(\mathcal{B}_d(r / 2)\right)}{\operatorname{Vol}\!\left(\mathbb{R}^d / \Lambda\right)} \cdot \frac{\operatorname{Vol}\!\left(\mathcal{B}_d(R + r / 2 + 2L)\right)}{\operatorname{Vol}\!\left(\mathcal{B}_d(R)\right)}$$
> 
> Taking limit on both sides as $R \to \infty$ and apply the Sandwich theorem and [[lemma-volume-ball-ratio-limit]], we get
> 
> $$\Delta_{\mathcal{P}} = \limsup_{R \to \infty} \Delta_{\mathcal{P}}(R) = \lim_{R \to \infty} \Delta_{\mathcal{P}}(R) = |X / \Lambda| \cdot \frac{\operatorname{Vol}\!\left(\mathcal{B}_d(r / 2)\right)}{\operatorname{Vol}\!\left(\mathbb{R}^d / \Lambda\right)}$$
