---
id: 98c36c6f7f77
type: lemma
---

# Lemma — lemma:psiI-psiT-psiS-fourier

## Statement

> [!lemma] lemma:psiI-psiT-psiS-fourier
> The Fourier expansions of these functions are
> $$
> \begin{aligned}
> \psi_I(z)\,=\,&q^{-1} + 144 + O(q^{1/2}) \\
> \psi_T(z)\,=\,&q^{-1} + 144 + O(q^{1/2}) 
> \end{aligned}
> $$

## Proof

> [!note]- Proof (click to expand)
> Work from the closed forms of [[lemma-psi-new]]: $\psi_I=\frac{H_4^3(5H_2^2+5H_2H_4+2H_4^2)}{2\Delta}$ and $\psi_T=\frac{H_3^3(5H_2^2-5H_2H_3+2H_3^2)}{2\Delta}$.
>
> Insert the theta expansions ([[def-th00-th01-th10]], [[def-h2-h3-h4]]): with $q=e^{2\pi iz}$,
> $$H_2=16q^{1/2}\,(1+q+\dots)^4,\qquad H_3=1+8q^{1/2}+24q+\dots,\qquad H_4=1-8q^{1/2}+24q-\dots,$$
> and $\Delta=q\prod_{n\ge1}(1-q^n)^{24}=q-24q^2+\dots$ ([[def-disc-definition]]).
>
> For $\psi_I$: the numerator is $H_4^3\big(5H_2^2+5H_2H_4+2H_4^2\big)=2+56q^{1/2}+\dots$, an expansion in $q^{1/2}$ with integer coefficients; dividing by $2\Delta=2q(1+\dots)$ shifts everything down by one power of $q$, so $\psi_I=q^{-1}+c_{1/2}q^{-1/2}+c_0+O(q^{1/2})$. Carrying the multiplication two steps further gives $c_{1/2}=0$ and $c_0=144$. The computation for $\psi_T$ is identical with $H_3$ in place of $H_4$ and the middle sign flipped, and yields the same two leading terms — as it must, since $\psi_T=\psi_I|_{-2}T$ ([[def-psii-psit-psis]]) and $T$ shifts $z$ by $1$, which multiplies the coefficient of $q^{n/2}$ by $e^{\pi in}$ and so fixes the $q^{-1}$ and $q^0$ terms.
>
> (Numerically, $\psi_I(it)-e^{2\pi t}\to 144$ and $\psi_T(it)-e^{2\pi t}\to 144$ as $t$ grows, through $103.3,\,134.7,\,142.0$ at $t=1.5,2,2.5$ — the $O(q^{1/2})$ tail is visibly $\sim e^{-\pi t}$.) These are the expansions behind [[eq-psii-near-infty]] and the growth bounds of [[lemma-psi-bound]]; cf. [[ref-via2017]], §6.

**Uses**: [[lemma-psi-new]].
