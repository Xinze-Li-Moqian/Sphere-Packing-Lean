---
id: 044af3957846
type: lemma
lean:
  - E_k_q_expansion
formalized: true
---

# Lemma — lemma:Ek-Fourier

## Statement

> [!lemma] lemma:Ek-Fourier
> The [[def-ek|Eisenstein series]] possesses the Fourier expansion
> $$E_k(z)=1+\frac{2}{\zeta(1-k)}\sum_{n=1}^\infty \sigma_{k-1}(n)\,e^{2\pi i n z}, $$
> where $\sigma_{k-1}(n)\,=\,\sum_{d|n} d^{k-1}$. In particular, we have
> $$
> \begin{aligned}
> E_4(z)\,=\,& 1+240\sum_{n=1}^\infty \sigma_3(n)\,e^{2\pi i n z} \notag \\
> E_6(z)\,=\,& 1-504\sum_{n=1}^\infty \sigma_5(n)\,e^{2\pi i n z}. \notag
> \end{aligned}
> $$

## Proof

> [!note]- Proof (click to expand)
> Start from the [[def-ek|defining sum]] over coprime pairs, $E_k(z)=\frac12\sum_{(c,d)=1}(cz+d)^{-k}$. Grouping all pairs by their gcd gives $\sum_{(c,d)\neq(0,0)}(cz+d)^{-k}=\zeta(k)\cdot 2E_k(z)$, so it suffices to expand the full lattice sum.
>
> The $c=0$ terms contribute $2\zeta(k)$. For each $c\ge 1$ the inner sum over $d$ is handled by the Lipschitz summation formula
> $$\sum_{d\in\mathbb{Z}}(w+d)^{-k}=\frac{(-2\pi i)^k}{(k-1)!}\sum_{m\ge1}m^{k-1}e^{2\pi i m w},\qquad w\in\mathfrak{H},$$
> itself a Poisson-summation identity — the same principle as [[thm-poisson-summation-formula]], applied in one variable. Setting $w=cz$ and summing over $c\ge1$, then collecting $e^{2\pi i mcz}$ by $n=mc$, produces $\sum_{n\ge1}\sigma_{k-1}(n)e^{2\pi inz}$ with the stated constant: dividing by $\zeta(k)$ and using the functional-equation value $\zeta(1-k)=\frac{2\,(k-1)!}{(-2\pi i)^k}\,\zeta(k)$ turns the prefactor into $2/\zeta(1-k)$.
>
> For $k=4$ and $k=6$: $\zeta(-3)=\frac1{120}$ and $\zeta(-5)=-\frac1{252}$, giving the coefficients $240$ and $-504$. Full details: [[ref-serre73]] VII.4, or [[ref-1-2-3]] Proposition 5.
>
> *(As imported, the exponent read $e^{2\pi i z}$ — the $n$ was missing. Corrected.)*

**Uses**: [[def-ek]].
