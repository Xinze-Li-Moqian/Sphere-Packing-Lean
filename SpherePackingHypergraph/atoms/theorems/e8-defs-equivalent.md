---
id: 30b96e609fb7
type: theorem
from: blueprint
lean:
  - span_E8Matrix
formalized: true
---

# Theorem — E8-defs-equivalent

## Statement

> [!theorem] E8-defs-equivalent
> The two definitions above coincide, i.e. $\Lambda_8 = \mathrm{span}_{\mathbb{Z}}(\mathcal{B}_8)$.

**In terms of**: [[e8-matrix]], [[e8-set]].

## Proof

> [!note]- Proof (click to expand)
> We prove each side contains the other side.
> 
> For a vector $\vec{v} \in \Lambda_8 \subseteq \mathbb{R}^8$, we have $\sum_i \vec{v}_i \equiv 0 \pmod{2}$ and $\vec{v}_i$ being either all integers or all half-integers. After some modulo arithmetic, it can be seen that $\mathcal{B}_8^{-1}\vec{v}$ as integer coordinates (i.e. it is congruent to $0$ modulo $1$). Hence, $\vec{v} \in \mathrm{span}_{\mathbb{Z}}(\mathcal{B}_8)$.
> 
> For the opposite direction, we write the vector as $\vec{v} = \sum_i c_i\mathcal{B}_8^i \in \mathrm{span}_{\mathbb{Z}}(\mathcal{B}_8)$ with $c_i$ being integers and $\mathcal{B}_8^i$ being the $i$-th basis vector. Expanding the definition then gives $\vec{v} = \left(c_1 - \frac{1}{2}c_7, -c_1 + c_2 - \frac{1}{2}c_7, \cdots, -\frac{1}{2}c_7\right)$. Again, after some modulo arithmetic, it can be seen that $\sum_i \vec{v}_i$ is indeed $0$ modulo $2$ and are all either integers and half-integers, concluding the proof.
> 
> (Note: this proof doesn't depend on that $\mathcal{B}_8$ is linearly independent.)

**Uses**: [[e8-matrix]], [[e8-set]].
