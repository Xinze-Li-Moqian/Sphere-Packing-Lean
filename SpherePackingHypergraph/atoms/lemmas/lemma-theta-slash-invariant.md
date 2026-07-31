---
id: fb60225446d1
type: lemma
from: blueprint
lean:
  - H₂_SIF
  - H₃_SIF
  - H₄_SIF
formalized: true
---

# Lemma — lemma:theta-slash-invariant

## Statement

> [!lemma] lemma:theta-slash-invariant
> $H_{2}$, $H_{3}$, and $H_{4}$ are slash invariant under $\Gamma(2)$, i.e. for all $\gamma \in \Gamma(2)$ and $i \in \{2, 3, 4\}$, we have $H_i|\gamma = H_i|\gamma^{-1} = H_i$.

**In terms of**: [[def-h2-h3-h4]].

## Proof

> [!note]- Proof (click to expand)
> By [[lemma-gamma-2-generators]] and [[lemma-slash-operator-chain-rule]], it suffices to show that the $H_i$ are invariant under slash actions with respect to $\alpha$, $\beta$, and $-I$.
> Invariance under $-I$ follows from Lemma [[lemma-slash-negi-even-weight]].
> The rest follows from Lemma [[lemma-slash-operator-chain-rule]], [[lemma-theta-transform-s-t]], and the matrix identities
> $$
> \alpha = T^2, \quad \beta = -S\alpha^{-1}S = -ST^{-2}S. 
> $$
> For example, invariance for $H_2$ can be proved by
> $$
> \begin{aligned}
> H_2|\alpha &= H_2 |T^{2} = -H_2 |T = H_2 \\
> H_2|\beta &= H_2 |(-S\alpha^{-1}S) = H_2 | (S\alpha^{-1}S) =-H_4 |(\alpha^{-1}S) = -H_4 |S  = H_2.
> \end{aligned}
> $$

**Uses**: [[lemma-gamma-2-generators]], [[lemma-slash-negi-even-weight]], [[lemma-slash-operator-chain-rule]], [[lemma-theta-transform-s-t]].
