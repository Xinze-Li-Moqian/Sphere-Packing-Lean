---
id: 01c64a89775e
type: lemma
lean:
  - volume_ball_ratio_tendsto_nhds_one''
formalized: true
---

# Lemma — lemma:volume-ball-ratio-limit

## Statement

> [!lemma] lemma:volume-ball-ratio-limit
> For any constant $C > 0$, we have
> 
> $$\lim_{R \to \infty} \frac{\mathrm{Vol}(\mathcal{B}_d(R))}{\mathrm{Vol}(\mathcal{B}_d(R + C))} = 1$$

## Proof

> [!note]- Proof (click to expand)
> Write out the formula for volume of a ball and simplify. More specifically, we have $\mathrm{Vol}(\mathcal{B}_d(R)) = R^d \pi^{d / 2} / \Gamma\left(\frac{d}{2} + 1\right)$, so $\mathrm{Vol}(\mathcal{B}_d(R)) / \mathrm{Vol}(\mathcal{B}_d(R + C)) = R^d / (R + C)^d = \left(1 - \frac{1}{R + C}\right)^d = 1$.
