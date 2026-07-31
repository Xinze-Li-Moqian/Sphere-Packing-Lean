---
id: 7f7809b9f984
type: theorem
---

# Theorem — thm:anti-serre-der-pos

## Statement

> [!theorem] thm:anti-serre-der-pos
> Let $F$ be a holomorphic quasimodular cusp form with real Fourier coefficients. Assume that there exists $k$ such that $(\partial_{k}F)(it) > 0$ for all $t > 0$. If the first Fourier coefficient of $F$ is positive, then $F(it) > 0$ for all $t > 0$.

## Proof

> [!note]- Proof (click to expand)
> By [[eq-logder-disc-e2]], we have
> $$
> \begin{aligned}
> \frac{\mathrm{d}}{\mathrm{d} t} \left( \frac{F(it)}{\Delta(it)^{\frac{k}{12}}}\right)
> &= (-2 \pi) \frac{F'(it) \Delta(it)^{\frac{k}{12}} - F(it) \frac{k}{12} E_{2}(it) \Delta(it)^{\frac{k}{12}}}{\Delta(it)^{\frac{k}{6}}} \\
> &= (-2 \pi) \frac{(\partial_{k} F)(it)}{\Delta(it)^{\frac{k}{12}}}  < 0,
> \end{aligned}
> $$
> hence
> 
> $$t \mapsto \frac{F(it)}{\Delta(it)^{\frac{k}{12}}}$$
> 
> is monotone decreasing. Because of the assumption on the positivity of the first nonzero Fourier coefficient of $F$, $F(it) > 0$ for sufficiently large $t$ since
> 
> $$F = \sum_{n \geq n_{0}} a_{n} q^{n} \Rightarrow e^{2 \pi n_{0} t} F(it) = a_{n_{0}} + e^{-2 \pi t}\sum_{n\geq n_{0} + 1} a_{n} e^{-2 \pi (n - n_{0} - 1)t}$$
> 
> and $\lim_{t \to \infty} e^{2 \pi n_{0}t} F(it) = a_{n_0} > 0$, hence the result follows.
