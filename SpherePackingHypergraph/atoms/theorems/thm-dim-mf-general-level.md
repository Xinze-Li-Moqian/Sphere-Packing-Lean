---
id: 9240553fc555
type: theorem
lean:
  - dim_gen_cong_levels
formalized: true
---

# Theorem — thm:dim-mf-general-level

## Statement

> [!theorem] thm:dim-mf-general-level
> Let $\Gamma$ be a [[def-congruence-subgroup|congruence subgroup]]. Then $M_k(\Gamma)$ is finite-dimensional.

## Proof

> [!note]- Proof (click to expand)
> We know that $\dim(M_k(\Gamma_1))$ is finite dimensional from the above, now this means that there is some $r_k$ such that any element of $M_k(\Gamma_1)$ vanishing at infinity to degree $> r_k$ must be zero. Now take $f \in M_k(\Gamma)$ and vanishes to degree $n$ at infinity, then consider $F = \prod_\gamma f\mid_k \gamma$ where the product is over a set of representatives of $\Gamma_1 \backslash \Gamma$. Then $F$ is a [[def-mk|modular form]] of weight $k d$ where $d = [\Gamma_1: \Gamma]$ and vanishes at infinity to degree at least $n$. So if $n > r_{kd}$ then $F=0$ meaning the $f=0$.
