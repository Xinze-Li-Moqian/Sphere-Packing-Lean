---
id: 65f54fa480cb
type: lemma
from: blueprint
---

# Lemma — lemma:psi-new

## Statement

> [!lemma] lemma:psi-new
> $\psi_I(z), \psi_S(z), \psi_T(z)$ can be written as
> $$
> \begin{aligned}
> \psi_I(z) &= \frac{H_4^3 (5 H_2^2 + 5 H_2 H_4 + 2 H_4^2)}{2\Delta},  \\
> \psi_S(z) &= -\frac{H_2^3 (2 H_2^2 + 5 H_2 H_4 + 5 H_4^2)}{2 \Delta}.  \\
> \psi_T(z) &= \frac{H_3^3 (5 H_2^2 - 5 H_2 H_3 + 2 H_3^2)}{2 \Delta}
> \end{aligned}
> $$

## Proof

> [!note]- Proof (click to expand)
> By Lemma [[lemma-theta-transform-s-t]], we have
> $$
> \begin{aligned}
> H_2|_{-2}ST = (-H_4)|_{-2}T = -H_3, \\
> H_3|_{-2}ST = (-H_3)|_{-2}T = -H_4, \\
> H_4|_{-2}ST = (-H_2)|_{-2}T = H_2.
> \end{aligned}
> $$
> Using these equations and Lemma [[lemma-lv1-lv2-identities]], we can rewrite $\psi_I(z)$ as
> $$
> \begin{aligned}
> \psi_I(z) &= h(z) - h|_{-2}ST(z) \\
> &= 128 \frac{H_3 + H_4}{H_2^2} - 128 \frac{-H_4 + H_2}{H_3^2} \\
> &= 128 \frac{H_3^2 (H_3 + H_4) - H_2^2 (H_2 - H_4)}{H_2^2 H_3^2} \\
> &= 128 \frac{(H_2 + H_4)^2 (H_2 + 2 H_4) - H_2^2 (H_2 - H_4)}{H_2^2 H_3^2} \\
> &= 128 \frac{H_4(5 H_2^2 + 5 H_2 H_4 + 2 H_4^2)}{ H_2^2 H_3^2} \\
> &= 128 \frac{H_4^3(5 H_2^2 + 5 H_2 H_4 + 2 H_4^2)}{ H_2^2 H_3^2 H_4^3} \\
> &= \frac{H_4^3 (5 H_2^2 + 5 H_2 H_4 + 2 H_4^2)}{2\Delta}.
> \end{aligned}
> $$
> Applying $|_{-2}S$ and $|_{-2}T$ to the expression of $\psi_I$ proves [[eq-psis-new]] and [[eq-psit-new]].
