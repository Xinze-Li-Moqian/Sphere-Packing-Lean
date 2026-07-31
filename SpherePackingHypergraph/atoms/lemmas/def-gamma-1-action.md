---
id: f12bc5e92955
type: lemma
from: blueprint
formalized: true
---

# Lemma — def:Gamma-1-Action

## Statement

> [!lemma] def:Gamma-1-Action
> The modular group $\Gamma_1:=\mathrm{SL}_2(\mathbb{Z})$ acts on $\mathfrak{H}$ by linear fractional transformations
> $$\left(\begin{smallmatrix}a&b\\c&d\end{smallmatrix}\right)z:=\frac{az+b}{cz+d}.$$

**Used by**: [[def-level-n-princ-cong-subgp]], [[def-slash-operator]], [[lemma-ek-is-modular-form]], [[lemma-theta-bounded-im-infty]].

## Proof

> [!note]- Proof (click to expand)
> 

## Notes

> [!note]- Notes (click to expand)
> - The action is by fractional linear maps, so $\pm I$ acts trivially and the group that really acts is $\mathrm{PSL}_2(\mathbb{Z})$; the sign is why weights in this development are even.
> - Two elements generate it — [[def-gamma-generators|$S$ and $T$]], $z \mapsto -1/z$ and $z \mapsto z+1$ — so a function invariant under both is invariant under everything, which is what makes [[def-mk|modularity]] a checkable condition.
> - $S$ is also what the [[def-fourier-transform|Fourier transform]] does to a Gaussian of parameter $z$: it returns one of parameter $-1/z$. Modularity in $z$ and Fourier behaviour in $x$ are the same statement, and that is the bridge the construction crosses.
> - Its [[def-congruence-subgroup|congruence subgroups]] are where the functions of this proof actually live.
