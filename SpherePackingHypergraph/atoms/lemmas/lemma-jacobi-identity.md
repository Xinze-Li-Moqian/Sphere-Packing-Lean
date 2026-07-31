---
id: 34537e3c3a08
type: lemma
lean:
  - jacobi_identity
formalized: true
---

# Lemma — lemma:jacobi-identity

## Statement

> [!lemma] lemma:jacobi-identity
> These three [[def-th00-th01-th10|theta functions]] satisfy the *Jacobi identity*
> $$
> H_{2} + H_{4} = H_{3} \Leftrightarrow \Theta_{2}^4 + \Theta_{4}^4 = \Theta_{3}^4.
> $$

## Proof

> [!note]- Proof (click to expand)
> Let $f = (H_2 + H_4 - H_3)^{2}$.
> Obviously, $f$ is a [[def-mk|modular form]] of weight $4$ and level $\Gamma(2)$.
> However, by using the transformation rules of $H_2, H_3, H_4$, one have
> $$
> \begin{aligned}
> f|_{S} &= (-H_4 - H_2 + H_3)^{2} = f\\
> f|_{T} &= (-H_2 + H_3 - H_4)^{2} = f
> \end{aligned}
> $$
> so $f$ is actually a modular form of level $1$.
> By considering the limit as $z \to i\infty$, $f$ is a cusp form, so we get $f = 0$ from [[eq-dims4]].
