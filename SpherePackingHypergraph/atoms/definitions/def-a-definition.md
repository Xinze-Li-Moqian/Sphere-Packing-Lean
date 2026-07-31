---
id: d76a819acb6e
type: definition
lean:
  - MagicFunction.a.RealIntegrals.a'
  - MagicFunction.a.RadialFunctions.a
formalized: true
---

# Definition — def:a-definition

## Statement

> [!definition] def:a-definition
> Define $a_{\mathrm{rad}} : \mathbb{R} \to \mathbb{C}$ by
> $$
> \begin{aligned}
> a_\mathrm{rad}(r) := I_1(r) + I_2(r) + I_3(r) + I_4(r) + I_5(r) + I_6(r)
> \end{aligned}
> $$
> where
> $$
> \begin{aligned}
> I_1(r) &:= \int_{-1}^{-1 + i} \phi_0 \left(\frac{-1}{z+1}\right) (z + 1)^2 e^{\pi i r z} \mathrm{d} z  \\
> I_2(r) &:= \int_{-1 + i}^{i} \phi_0 \left(\frac{-1}{z+1}\right) (z + 1)^2 e^{\pi i r z} \mathrm{d} z  \\
> I_3(r) &:= \int_{1}^{1 + i} \phi_0 \left(\frac{-1}{z-1}\right) (z - 1)^2 e^{\pi i r z} \mathrm{d} z  \\
> I_4(r) &:= \int_{1 + i}^{i} \phi_0 \left(\frac{-1}{z-1}\right) (z - 1)^2 e^{\pi i r z} \mathrm{d} z  \\
> I_5(r) &:= -2 \int_{0}^{i} \phi_0 \left(\frac{-1}{z}\right) z^2 e^{\pi i r z} \mathrm{d} z  \\
> I_6(r) &:= 2 \int_{i}^{i\infty} \phi_0(z) e^{\pi i r z} \mathrm{d} z 
> \end{aligned}
> $$
> Here all the contours are chosen to be straight line segments.
> Now, define $a(x) := a_{\mathrm{rad}}(\|x\|^2)$ for $x \in \mathbb{R}^8$.
