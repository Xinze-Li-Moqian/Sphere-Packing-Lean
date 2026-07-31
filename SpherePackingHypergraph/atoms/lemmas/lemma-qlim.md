---
id: e70cf8682c51
type: lemma
from: blueprint
lean:
  - FmodG_rightLimitAt_zero
formalized: true
---

# Lemma — lemma:Qlim

## Statement

> [!lemma] lemma:Qlim
> We have
> $$
> \lim_{t \to 0^+} Q(t) = \frac{18}{\pi^2}.
> $$

## Proof

> [!note]- Proof (click to expand)
> We have
> $$
> \lim_{t \to 0^+} Q(t) = \lim_{t \to 0^+} \frac{F(it)}{G(it)} = \lim_{t \to \infty} \frac{F(i/t)}{G(i/t)}.
> $$
> By using the transformation laws of [[def-ek|Eisenstein series]] [[eq-e2-s-transform]], [[eq-ek-trans-s]] (for $k = 4, 6$) and the thetanull functions, [[eq-h2-transform-s]], [[eq-h4-transform-s]], we get
> $$
> \begin{aligned}
> F\left(\frac{i}{t}\right) &= t^{12} F(it) - \frac{12t^{11}}{\pi} (E_2(it)E_4(it) - E_6(it))E_4(it) + \frac{36t^{10}}{\pi^2}E_4(it)^2, \\
> G\left(\frac{i}{t}\right) &= t^{10} H_{4}(it)^{3}(2H_{4}(it)^{2} + 5 H_{4}(it)H_{2}(it) + 5 H_{2}(it)^{2}).
> \end{aligned}
> $$
> Since $F$, $E_2 E_4 - E_6$ and $H_2$ are [[def-cusp-form|cusp forms]], we have $\lim_{t \to \infty}t^k A(it) = 0$ when $A(z)$ is one of these forms and $k \geq 0$.
> From $\lim_{t \to \infty} E_4(it) = 1 = \lim_{t \to \infty}H_{4}(it)$, we get
> $$
> \begin{aligned}
> \lim_{t \to \infty} \frac{F(i/t)}{G(i/t)}
> &= \lim_{t \to \infty} \frac{t^{12} F(it) - \frac{12t^{11}}{\pi} (E_2(it)E_4(it) - E_6(it))E_4(it) + \frac{36t^{10}}{\pi^2}E_4(it)^2}{t^{10} H_{4}(it)^{3}(2H_{4}(it)^{2} + 5 H_{4}(it)H_{2}(it) + 5 H_{2}(it)^{2})} \\
> &= \lim_{t \to \infty} \frac{t^{2} F(it) - \frac{12t}{\pi} (E_2(it)E_4(it) - E_6(it))E_4(it) + \frac{36}{\pi^2}E_4(it)^2}{H_{4}(it)^{3}(2H_{4}(it)^{2} + 5 H_{4}(it)H_{2}(it) + 5 H_{2}(it)^{2})} \\
> &= \frac{18}{\pi^2}.
> \end{aligned}
> $$
