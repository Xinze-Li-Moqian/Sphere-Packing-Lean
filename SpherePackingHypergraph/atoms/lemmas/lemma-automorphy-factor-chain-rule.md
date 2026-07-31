---
id: b636bcf78d6b
type: lemma
lean:
  - UpperHalfPlane.denom_cocycle
formalized: true
---

# Lemma — lemma:automorphy-factor-chain-rule

## Statement

> [!lemma] lemma:automorphy-factor-chain-rule
> The [[def-automorphy-factor|automorphy factor]] satisfies the *chain rule*
> $$j_k(z,\gamma_1\gamma_2)=j_k(z,\gamma_2)\,j_k(\gamma_2z,\gamma_1). $$

## Proof

> [!note]- Proof (click to expand)
> Write $J(\gamma,z):=cz+d$ for the bottom row of $\gamma$, so that $j_k(z,\gamma)=J(\gamma,z)^{-k}$ by [[def-automorphy-factor]]. It suffices to prove the cocycle identity
> $$J(\gamma_1\gamma_2,z)=J(\gamma_1,\gamma_2 z)\,J(\gamma_2,z),$$
> and then raise it to the power $-k$.
>
> With $\gamma_1=\left(\begin{smallmatrix}a&b\\c&d\end{smallmatrix}\right)$, $\gamma_2=\left(\begin{smallmatrix}e&f\\g&h\end{smallmatrix}\right)$, the bottom row of $\gamma_1\gamma_2$ is $(ce+dg,\;cf+dh)$, so
> $$J(\gamma_1\gamma_2,z)=(ce+dg)z+(cf+dh).$$
> On the other side, using [[def-gamma-1-action]] for $\gamma_2 z$:
> $$J(\gamma_1,\gamma_2 z)\,J(\gamma_2,z)=\left(c\,\frac{ez+f}{gz+h}+d\right)(gz+h)=c(ez+f)+d(gz+h)=(ce+dg)z+(cf+dh).$$
> The two agree, and raising to $-k$ gives $j_k(z,\gamma_1\gamma_2)=j_k(\gamma_2z,\gamma_1)\,j_k(z,\gamma_2)$ as claimed.
>
> *(As imported, the statement read $j_k(z,\gamma_1)$ for the first factor — a typo: the two sides then disagree already for $\gamma_1=\left(\begin{smallmatrix}2&1\\1&1\end{smallmatrix}\right)$, $\gamma_2=\left(\begin{smallmatrix}1&1\\1&2\end{smallmatrix}\right)$ at $z=0.3+1.7i$. Corrected here.)*

**Uses**: [[def-automorphy-factor]].
