---
id: 01984b3a8cc6
type: proposition
lean:
  - FmodG_strictAntiOn
formalized: true
---

# Proposition — prop:Qdec

## Statement

> [!proposition] prop:Qdec
> The function $t \mapsto Q(t)$ is strictly decreasing.

## Proof

> [!note]- Proof (click to expand)
> It is enough to show that
> $$
> \begin{aligned}
> \frac{\mathrm{d}}{\mathrm{d} t} \left(\frac{F(it)}{G(it)}\right) < 0 &\Leftrightarrow (- 2\pi) \frac{F'(it)G(it) - F(it) G'(it)}{G(it)^{2}} < 0 \\
> &\Leftrightarrow F'(it) G(it) - F(it) G'(it) > 0 \\
> &\Leftrightarrow (\partial_{10}F)(it) G(it) - F(it) (\partial_{10}G)(it) > 0.
> \end{aligned}
> $$
> Let $\mathcal{L}_{1, 0} := (\partial_{10}F) G - F (\partial_{10} G) = F'G - FG'$.
> Then
> $$
> \begin{aligned}
> \frac{\mathcal{L}_{1, 0}}{FG} = \frac{F'G - FG'}{FG} = \frac{F'}{F} - \frac{G'}{G}
> \end{aligned}
> $$
> The vanishing order of $F$ and $G$ at the infinity are $2$ and $\frac{3}{2}$ respectively, so by Lemma [[lemma-log-der-inf]], we have
> $$
> \begin{aligned}
> \lim_{t \to \infty} \frac{\mathcal{L}_{1, 0}(it)}{F(it) G(it)} = \lim_{t \to \infty} \left(\frac{F'(it)}{F(it)} - \frac{G'(it)}{G(it)}\right) = 2 - \frac{3}{2} = \frac{1}{2} > 0
> \end{aligned}
> $$
> so $\mathcal{L}_{1, 0}(it) > 0$ for sufficiently large $t$.
> Its [[def-serre-der|Serre derivative]] $\partial_{22} \mathcal{L}_{1, 0}$ is positive by Corollary [[cor-mlde-pos]]:
> $$
> \begin{aligned}
> \partial_{22} \mathcal{L}_{1, 0} = (\partial_{12} \partial_{10} F) G - F (\partial_{12}\partial_{10} G)
> = \Delta (7200 (-E_{2}') G + 640 H_2 F) > 0.
> \end{aligned}
> $$
> Hence $\mathcal{L}_{1, 0}(it) > 0$ by Theorem [[thm-anti-serre-der-pos]], and the monotonicity follows.
