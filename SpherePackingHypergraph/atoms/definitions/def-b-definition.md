---
id: 5b7b3dba94c0
type: definition
from: blueprint
---

# Definition — def:b-definition

## Statement

> [!definition] def:b-definition
> Define $b_\mathrm{rad} : \mathbb{R} \to \mathbb{C}$ by
> $$
> 
> b_\mathrm{rad}(r) := J_1(r) + J_2(r) + J_3(r) + J_4(r) + J_5(r) + J_6(r)
> $$
> where for $r \in \mathbb{R}$,
> $$
> \begin{aligned}
> J_1(r) &:= \int_{-1}^{-1 + i} \psi_T(z) e^{\pi i r z} \, \mathrm{d} z,  \\
> J_2(r) &:= \int_{-1 + i}^{i} \psi_T(z) e^{\pi i r z} \, \mathrm{d} z,  \\
> J_3(r) &:= \int_{1}^{1 + i} \psi_T(z) e^{\pi i r z} \, \mathrm{d} z,  \\
> J_4(r) &:= \int_{1 + i}^{i} \psi_T(z) e^{\pi i r z} \, \mathrm{d} z,  \\
> J_5(r) &:= -2 \int_{0}^{i} \psi_I(z) e^{\pi i r z} \, \mathrm{d} z,  \\
> J_6(r) &:= -2 \int_{i}^{i \infty} \psi_S(z) e^{\pi i r z} \, \mathrm{d} z. 
> \end{aligned}
> $$
> Here all the contours are straight line segments.
> Then we define $b : \mathbb{R}^8 \to \mathbb{C}$ by $b(x) := b_\mathrm{rad}(\|x\|^2)$.

**Uses**: [[def-psii-psit-psis]].
