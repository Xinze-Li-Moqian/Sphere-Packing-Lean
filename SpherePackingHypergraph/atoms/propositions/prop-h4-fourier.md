---
id: ef21dc184690
type: proposition
---

# Proposition — prop:H4-fourier

## Statement

> [!proposition] prop:H4-fourier
> $H_4$ admits a Fourier series of the form
> $$
> H_4(z) = \sum_{n \ge 0} c_{H_4}(n) e^{\pi i n z}
> $$
> for some $c_{H_4}(n) \in \mathbb{R}$ with $c_{H_4}(0) = 1$ and $c_{H_4}(n) = O(n^k)$ for some $k \in \mathbb{N}$.
> Especially, $H_4$ is not cuspidal.

## Proof

> [!note]- Proof (click to expand)
> By [[def-h2-h3-h4|the definition]] and [[def-th00-th01-th10|that of the theta functions]], $H_4=\Theta_4^4$ with $\Theta_4(z)=\sum_{n\in\mathbb{Z}}(-1)^n e^{\pi in^2z}$. Multiplying four copies and collecting exponents:
> $$H_4(z)=\sum_{n\ge0}c_{H_4}(n)\,e^{\pi inz},\qquad c_{H_4}(n)=(-1)^n r_4(n),$$
> where $r_4(n)=\#\{(a,b,c,d)\in\mathbb{Z}^4:a^2+b^2+c^2+d^2=n\}$ — the sign is $(-1)^{a+b+c+d}$, and $a+b+c+d\equiv a^2+b^2+c^2+d^2=n\pmod 2$.
>
> The three claims read off: $c_{H_4}(0)=r_4(0)=1$. Every coefficient is an integer, in particular real. And by Jacobi&#8217;s four-square theorem $r_4(n)=8\sum_{4\nmid d\mid n}d\le 8\sigma(n)=O(n\log n)=O(n^2)$, so the coefficients grow polynomially ([[ref-mumford]] I.\S3 for the theta identities, or [[ref-1-2-3]] \S3).
>
> Since $c_{H_4}(0)=1\neq0$, $H_4$ does not vanish at the cusp $i\infty$ — it is not [[def-cusp-form|cuspidal]].

**Uses**: [[def-h2-h3-h4]].
