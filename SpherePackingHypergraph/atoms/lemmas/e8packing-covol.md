---
id: 7e354474e8e5
type: lemma
lean:
  - E8Basis_volume
formalized: true
---

# Lemma — E8Packing-covol

## Statement

> [!lemma] E8Packing-covol
> $\operatorname{Vol}\!\left(\Lambda_8\right) = \mathrm{Covol}(\mathbb{R}^8 / \Lambda_8) = 1$.

**In terms of**: [[e8-set]].

## Proof

> [!note]- Proof (click to expand)
> The covolume of a full-rank [[iszlattice|lattice]] is $|\det M|$ for any matrix $M$ whose columns are a $\mathbb{Z}$-basis, and by [[e8-defs-equivalent]] the columns of [[e8-matrix|$\mathcal{B}_8$]] are such a basis for $\Lambda_8$.
>
> So it remains to compute $\det\mathcal{B}_8$. The first five columns are the chain $e_1-e_2,\,e_2-e_3,\,e_3-e_4,\,e_4-e_5,\,e_5-e_6$; the sixth and eighth are $e_6+e_7$ and $e_6-e_7$; only the seventh, $v_7=(-\tfrac12,\dots,-\tfrac12)$, has a nonzero last coordinate. Expanding along the eighth row leaves $-\tfrac12$ times the $7\times 7$ determinant of the remaining columns in coordinates $1..7$, and eliminating along the chain reduces that to $\det\left(\begin{smallmatrix}1&1\\1&-1\end{smallmatrix}\right)=-2$ in coordinates $6,7$. Altogether $\det\mathcal{B}_8=(-\tfrac12)\cdot(-2)\cdot(\pm1)=-1$; exact rational elimination confirms the value $-1$.
>
> Hence $\mathrm{Covol}(\mathbb{R}^8/\Lambda_8)=|\det\mathcal{B}_8|=1$: the lattice is unimodular. This is also forced by self-duality, since a lattice and its [[def-dual-lattice|dual]] have reciprocal covolumes.

**Uses**: [[e8packing]].
