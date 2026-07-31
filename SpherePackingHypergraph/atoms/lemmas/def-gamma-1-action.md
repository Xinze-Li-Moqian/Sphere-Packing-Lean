---
id: f12bc5e92955
type: lemma
formalized: true
---

# Lemma — def:Gamma-1-Action

## Statement

> [!lemma] def:Gamma-1-Action
> The modular group $\Gamma_1:=\mathrm{SL}_2(\mathbb{Z})$ acts on $\mathfrak{H}$ by linear fractional transformations
> $$\left(\begin{smallmatrix}a&b\\c&d\end{smallmatrix}\right)z:=\frac{az+b}{cz+d}.$$

**Used by**: [[def-level-n-princ-cong-subgp]], [[def-slash-operator]], [[lemma-ek-is-modular-form]], [[lemma-theta-bounded-im-infty]].

> Three things need checking: that the formula lands in $\mathfrak{H}$, that the identity acts trivially, and that composition of maps matches multiplication of matrices.
>
> For the first, a direct computation with $\gamma=\left(\begin{smallmatrix}a&b\\c&d\end{smallmatrix}\right)$, $ad-bc=1$:
> $$\Im(\gamma z)=\Im\frac{(az+b)(c\bar z+d)}{|cz+d|^2}=\frac{(ad-bc)\,\Im z}{|cz+d|^2}=\frac{\Im z}{|cz+d|^2}>0,$$
> and $cz+d\neq 0$ because $z\notin\mathbb{R}$ while $-d/c\in\mathbb{R}$. So $\gamma z\in\mathfrak{H}$.
>
> The identity matrix gives $z\mapsto\frac{z+0}{0+1}=z$.
>
> For composition, write $\gamma_1=\left(\begin{smallmatrix}a&b\\c&d\end{smallmatrix}\right)$, $\gamma_2=\left(\begin{smallmatrix}e&f\\g&h\end{smallmatrix}\right)$ and expand both sides on a common denominator:
> $$\gamma_1(\gamma_2 z)=\frac{a\frac{ez+f}{gz+h}+b}{c\frac{ez+f}{gz+h}+d}=\frac{(ae+bg)z+(af+bh)}{(ce+dg)z+(cf+dh)}=(\gamma_1\gamma_2)z,$$
> the middle step multiplying through by $gz+h$ and the last reading off the entries of the matrix product. Note $-I$ acts trivially, so the action factors through $\mathrm{PSL}_2(\mathbb{Z})$. See [[ref-first-course]], §1.1.

## Proof

> [!note]- Proof (click to expand)
> Three things need checking: that the formula lands in $\mathfrak{H}$, that the identity acts trivially, and that composition of maps matches multiplication of matrices.
>
> For the first, a direct computation with $\gamma=\left(\begin{smallmatrix}a&b\\c&d\end{smallmatrix}\right)$, $ad-bc=1$:
> $$\Im(\gamma z)=\Im\frac{(az+b)(c\bar z+d)}{|cz+d|^2}=\frac{(ad-bc)\,\Im z}{|cz+d|^2}=\frac{\Im z}{|cz+d|^2}>0,$$
> and $cz+d\neq 0$ because $z\notin\mathbb{R}$. So $\gamma z\in\mathfrak{H}$.
>
> The identity matrix gives $z\mapsto\frac{z+0}{0+1}=z$.
>
> For composition, write $\gamma_1=\left(\begin{smallmatrix}a&b\\c&d\end{smallmatrix}\right)$, $\gamma_2=\left(\begin{smallmatrix}e&f\\g&h\end{smallmatrix}\right)$ and expand both sides on a common denominator:
> $$\gamma_1(\gamma_2 z)=\frac{a\frac{ez+f}{gz+h}+b}{c\frac{ez+f}{gz+h}+d}=\frac{(ae+bg)z+(af+bh)}{(ce+dg)z+(cf+dh)}=(\gamma_1\gamma_2)z,$$
> the middle step multiplying through by $gz+h$ and the last reading off the entries of the matrix product. Note $-I$ acts trivially, so the action factors through $\mathrm{PSL}_2(\mathbb{Z})$. See [[ref-first-course]], §1.1.

## Notes

> [!note]- Notes (click to expand)
> - The action is by fractional linear maps, so $\pm I$ acts trivially and the group that really acts is $\mathrm{PSL}_2(\mathbb{Z})$; the sign is why weights in this development are even.
> - Two elements generate it — [[def-gamma-generators|$S$ and $T$]], $z \mapsto -1/z$ and $z \mapsto z+1$ — so a function invariant under both is invariant under everything, which is what makes [[def-mk|modularity]] a checkable condition.
> - $S$ is also what the [[def-fourier-transform|Fourier transform]] does to a Gaussian of parameter $z$: it returns one of parameter $-1/z$. Modularity in $z$ and Fourier behaviour in $x$ are the same statement, and that is the bridge the construction crosses.
> - Its [[def-congruence-subgroup|congruence subgroups]] are where the functions of this proof actually live.
