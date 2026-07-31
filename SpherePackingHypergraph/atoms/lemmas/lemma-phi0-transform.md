---
id: 3d5e64c9e9de
type: lemma
---

# Lemma — lemma:phi0-transform

## Statement

> [!lemma] lemma:phi0-transform
> We have
> $$
> \begin{aligned}
> \phi_0(z + 1) &= \phi_0(z)  \\
> \phi_0\left(-\frac{1}{z}\right) &= \phi_0(z)-\frac{12i}{\pi}\,\frac{1}{z}\,\phi_{-2}(z)-\frac{36}{\pi^2}\,\frac{1}{z^2}\,\phi_{-4}(z).
> \end{aligned}
> $$

## Proof

> [!note]- Proof (click to expand)
> [[eq-phi0-trans-t]] easily follows from periodicity of [[def-ek|Eisenstein series]] and $\Delta(z)$.
> For [[eq-phi0-trans-s]],
> $$
> \begin{aligned}
> \phi_{0}\left(-\frac{1}{z}\right) &= \frac{(E_2(-1/z) E_4(-1/z) - E_6(-1/z))^{2}}{\Delta(-1/z)} \\
> &= \frac{((z^2 E_2(z) - 6iz / \pi) \cdot z^4 E_4(z) - z^6 E_6(z))^{2}}{z^{12} \Delta(z)} \\
> &= \frac{\left(E_2(z) E_4(z) - E_6(z) - \frac{6i}{\pi z} E_4(z)\right)^2}{\Delta(z)} \\
> &= \frac{(E_2(z) E_4(z) - E_6(z))^{2} - \frac{12i}{\pi z}(E_2(z) E_4(z) - E_6(z)) E_4(z) - \frac{36}{\pi^2 z^2} E_4(z)^{2}}{\Delta(z)} \\
> &= \phi_0(z) - \frac{12 i}{\pi z} \phi_{-2}(z) - \frac{36}{\pi^2 z^2} \phi_{-4}(z).
> \end{aligned}
> $$
