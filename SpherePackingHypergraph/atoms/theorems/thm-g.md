---
id: 4c34b8f1bd46
type: theorem
---

# Theorem — thm:g

## Statement

> [!theorem] thm:g
> There exists a radial [[def-schwartz-space|Schwartz function]] $g:\mathbb{R}^8\to\mathbb{R}$ which satisfies:
> $$
> \begin{aligned}
> g(x)&\leq 0\mbox{ for } \|x\|\geq \sqrt{2} \\
> \widehat{g}(x)&\geq0\mbox{ for all } x\in\mathbb{R}^8\\
> g(0)&=\widehat{g}(0)=1.
> \end{aligned}
> $$

## Proof

> [!note]- Proof (click to expand)
> Take the explicit function of [[thm-g1]]:
> $$g(x)=\frac{\pi i}{8640}\,a(x)+\frac{i}{240\pi}\,b(x).$$
>
> **It is a radial Schwartz function**: $a$ and $b$ are built as $a_{\mathrm{rad}}(\|x\|^2)$, $b_{\mathrm{rad}}(\|x\|^2)$ ([[def-a-definition]], [[def-b-definition]]), and are Schwartz by [[prop-a-schwartz]] and [[prop-b-schwartz]] — both through the criterion [[thm-smooth-fast-decay-schwartz]].
>
> **It is real-valued**: by the integral representations [[prop-a-another-integral]] and [[prop-b-another-integral]], $a(r)$ and $b(r)$ are $4i$ times real quantities — $\phi_0$ and $\psi_I$ have real $q$-coefficients, so are real on the imaginary axis — hence $ia$ and $ib$ are real, and so are the two coefficients times $i$.
>
> **The three conditions** are [[eq-g1]], [[eq-g2]], [[eq-g3]], proven for this $g$ in [[thm-g1]]: the sign of $g$ beyond $\sqrt2$ comes from [[prop-ineqa]] through the factorization with $\sin^2(\pi r^2/2)$, the sign of $\widehat g$ from [[prop-ineqb]] together with the eigenfunction relations [[prop-a-fourier]] and [[prop-b-fourier]], and the normalization $g(0)=\widehat g(0)=1$ from the values [[prop-a0]] and [[prop-b0]].
>
> This is the magic function of [[ref-via2017]], Theorem 1 — the certificate that [[thm-cohn-elkies-general|the Cohn–Elkies bound]] is exact in dimension eight.

**Uses**: [[thm-g1]].
