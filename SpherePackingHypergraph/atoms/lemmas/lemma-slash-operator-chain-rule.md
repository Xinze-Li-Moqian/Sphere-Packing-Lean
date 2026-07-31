---
id: 465aee36eca4
type: lemma
lean:
  - SlashAction.slash_mul
formalized: true
---

# Lemma — lemma:slash-operator-chain-rule

## Statement

> [!lemma] lemma:slash-operator-chain-rule
> The chain rule implies $$F|_k\gamma_1\gamma_2=(F|_k\gamma_1)|_k\gamma_2.$$

**In terms of**: [[def-slash-operator]].

## Proof

> [!note]- Proof (click to expand)
> Unfold [[def-slash-operator|the slash operator]] twice and once:
> $$\big((F|_k\gamma_1)|_k\gamma_2\big)(z)=j_k(z,\gamma_2)\,(F|_k\gamma_1)(\gamma_2 z)=j_k(z,\gamma_2)\,j_k(\gamma_2 z,\gamma_1)\,F\big(\gamma_1(\gamma_2 z)\big).$$
> By [[lemma-automorphy-factor-chain-rule]] the product of the two automorphy factors is $j_k(z,\gamma_1\gamma_2)$, and by [[def-gamma-1-action]] $\gamma_1(\gamma_2z)=(\gamma_1\gamma_2)z$. So the right-hand side is exactly $\big(F|_k(\gamma_1\gamma_2)\big)(z)$.
>
> In particular the slash is a right action of $\Gamma_1$, which is what lets [[def-mk|modularity]] be checked on the two generators [[def-gamma-generators|$S$ and $T$]] alone.

**Uses**: [[lemma-automorphy-factor-chain-rule]].
