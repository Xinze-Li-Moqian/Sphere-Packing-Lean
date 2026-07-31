---
topic: sphere-packing-lean
type: topic
section: "5"
prose: narrative/05.md
---

# Modular forms

Nothing in this section mentions sphere packing. It is the toolbox, and the reason it is *this* toolbox is worth stating before the tools.

## Why modular forms turn up at all

The function needed at the end has to satisfy a condition relating $f$ to $\hat f$. Such conditions are hard to impose directly — the Fourier transform is an integral, and prescribing what it does at infinitely many points is not something one does by adjusting coefficients.

The way in is the Gaussian. For $z$ in the upper half plane, the function $x \mapsto e^{\pi i \|x\|^2 z}$ has a Fourier transform which is another Gaussian, of parameter $-1/z$. So the Fourier transform, restricted to this family, *acts by* $z \mapsto -1/z$.

That map is one of the two generators of the modular group. A function of $z$ that transforms predictably under $z \mapsto -1/z$ therefore produces, after integrating against the Gaussian family, a function of $x$ that transforms predictably under the Fourier transform. **Modularity in $z$ becomes Fourier behaviour in $x$** — and that is why a problem about packings in $\mathbb{R}^8$ is solved with objects from the theory of modular forms.

## What is collected here

The tools are the standard ones, gathered because the construction uses them in a specific combination.

The group $\mathrm{SL}_2(\mathbb{Z})$ and its congruence subgroups $\Gamma(2)$, with generators, so that a transformation law can be checked on two elements instead of infinitely many. The slash operator, which is bookkeeping for "transforms with weight $k$".

Eisenstein series $E_k$, the discriminant $\Delta$, the Dedekind $\eta$ function, and the dimension counts that make the space of forms of a given weight finite — which is what makes the eventual construction a matter of writing down a specific combination rather than searching.

Theta functions $\theta_{00}, \theta_{01}, \theta_{10}$ and the forms $H_2, H_3, H_4$ built from them. These carry level $2$ structure, which is where the $\sqrt{2n}$ spacing of $E_8$ will come from: a $q$-expansion in integer powers becomes a function vanishing at those radii and no others.

$E_2$ and the Serre derivative. $E_2$ is *quasi*modular — its transformation law has an extra term — and that defect is not a nuisance to be avoided but the source of the inhomogeneity the construction needs. The Serre derivative is differentiation corrected so that it maps modular forms to modular forms, and Ramanujan's formulas say how the standard forms differentiate.


In this section, we recall and develop some theory of (quasi)modular forms.


## Modular forms and examples


Let $\mathfrak{H}$ be the upper half-plane $\{z\in\mathbb{C}\mid\Im(z)>0\}$.

![[def-gamma-1-action]]

Let $N$ be a positive integer.

![[def-level-n-princ-cong-subgp]]

![[def-congruence-subgroup]]

![[def-gamma-generators]]

The following two lemmas tell us the group structure of $\Gamma(1) = \Gamma_1$ and $\Gamma(2)$, which we will use later on to define the theta forms.

![[lemma-gamma-1-generators]]

![[lemma-gamma-2-generators]]

Let $z\in\mathfrak{H}$, $k\in\mathbb{Z}$, and $\left(\begin{smallmatrix}a&b\\c&d\end{smallmatrix}\right)\in\mathrm{SL}_2(\mathbb{Z})$. We omit many of the proofs below when they exist in Mathlib already.

![[def-automorphy-factor]]

![[lemma-automorphy-factor-chain-rule]]

![[def-slash-operator]]

![[lemma-slash-operator-chain-rule]]

In particular, this lemma implies that if $\Gamma = \langle M_i \rangle_{i \in \mathcal{I}} \rangle$, then the slash action $F|\gamma$ is uniquely determined by the action of generators, i.e. $F|M_i$ and $F|M_i^{-1}$.

![[lemma-slash-negi-even-weight]]

![[def-mk]]

By replacing condition $(3)$ above with (4) below defines the subspace of cusp forms, which we denote by $S_k(\Gamma)$.

1. For all $\gamma \in \mathrm{SL}_2(\mathbb{Z})$, and all  $0 < \epsilon$, there exists $A \in \mathbb{R}$ such that for all $z \in \mathbb{H}$, with $ A \le \mathrm{Im}(z)$, we have $|(f \mid_k \gamma) (z) |\le \epsilon$.

Let us consider several examples of modular forms.

![[def-ek]]

![[lemma-ek-is-modular-form]]

Since modular forms are holomorphic and periodic they have a Fourier expansions. One thing that we will need is the growth of the Fourier coefficients, which is given by the following lemma.

![[lemma-mod-form-poly-growth]]

For Eisenstein series, we can see this directly from the following:

![[lemma-ek-fourier]]

The infinite sum [[eq-ek-definition]] does not converge absolutely for $k=2$. On the other hand, the expression [[eq-ek-fourier]] converges to a holomorphic function on the upper half-plane and we will take it as a definition of $E_2$ (See Definition [[def-e2]] below).

The discriminant form is a unique normalized cusp form of weight 12, which can be defined as:

![[def-disc-definition]]

This product formula allows us to prove positivity of $\Delta(it)$ for $t > 0$ later. But we need to first check its a modular form. For this we first need some definitions/ results.

We define it as a $q$-series, which gives a holomorphic function on $\mathfrak{H}$.

![[def-e2]]

![[lemma-e2-transform-s]]

More generally, we have

![[lemma-e2-transform-general]]

![[def-dedekind-eta]]

![[lemma-dedekind-eta-transformation]]

![[lemma-disc-cuspform]]

![[lemma-disc-e4e6]]

![[cor-disc-pos]]

The following nonvanishing result, which directly follows from [[def-disc-definition]], will be used in the construction of the magic function.

![[cor-disc-nonvanishing]]

A key fact in the theory of modular forms is that the spaces $M_k(\Gamma)$ are finite-dimensional. To prove this we will do use the following non-standard proof. First we have the following result.

![[thm-nonpos-wt]]

![[thm-lvl1-dims]]

![[thm-dim-mf-general-level]]

![[cor-dim-mf]]

Another examples of modular forms we would like to consider are *theta functions* [[ref-1-2-3]].

![[def-th00-th01-th10]]

For convenience, we use the following notations for the fourth powers of the theta functions.

![[def-h2-h3-h4]]

Note that we only need these fourth powers to define [[def-b-definition]].

The group $\Gamma_1$ is generated by the elements $T=\left(\begin{smallmatrix}1&1\\0&1\end{smallmatrix}\right)$, $S=\left(\begin{smallmatrix}0&1\\-1&0\end{smallmatrix}\right)$, and $-I = \left(\begin{smallmatrix}-1&0\\0&-1\end{smallmatrix}\right)$ ([[lemma-gamma-1-generators]]), and the transformation of functions under $\Gamma(2)$ is determined by that under $\Gamma_1$ (by [[lemma-slash-operator-chain-rule]]).
The following lemma shows how the theta functions (and their powers) transform under the slash action of these matrices.

![[lemma-theta-transform-s-t]]

Using the above identities, we can prove that these are modular forms.

![[lemma-theta-slash-invariant]]

![[lemma-theta-bounded-im-infty]]

![[lemma-theta-modular]]

They have Fourier expansions as follows.

![[prop-h2-fourier]]

![[prop-h3-fourier]]

![[prop-h4-fourier]]

We also have a nontrivial relation between these theta functions.

![[lemma-jacobi-identity]]

These are also related to $E_4$, $E_6$, and $\Delta$ as follows.

![[lemma-lv1-lv2-identities]]

The *strict* positivity of Jacobi theta functions might needed later.

![[cor-theta-pos]]

## Quasimodular forms and derivatives


Morally, quasimodular forms can be thought as *modular forms with differentiations*.
It can be defined formally as follows:
Let $f: \mathfrak{H} \to \mathbb{C}$ be a holomorphic function, and let $k$ and $s \ge 0$ be integers.
The function $f$ is a *quasimodular form of weight $k$, level $\Gamma$, and depth $s$* if there exist holomorphic functions $f_0, \dots, f_s : \mathfrak{H} \to \mathbb{C}$ such that
$$
(f|_{k}\gamma)(z) = (cz + d)^{-k} f\left(\frac{az + b}{cz + d}\right) = \sum_{j=0}^{s} f_j(z) \left(\frac{c}{cz + d}\right)^j
$$
for all $z \in \mathfrak{H}$ and $\gamma = \left(\begin{smallmatrix} a&b\\c&d \end{smallmatrix}\right) \in \Gamma$.

By taking $\gamma = \left(\begin{smallmatrix} 1 & 0 \\ 0 & 1 \end{smallmatrix}\right)$, one can check that we should have $f_0 = f$. Thus, a quasimodular form of depth $0$ is just a modular form of same weight and level.
Also, it is easy to see that the space of quasimodular forms is closed under the normalized derivative.

In this project, we are *not* going to formalize the above definition of quasimodular forms. Instead, we only use $E_2$ (defined in [[def-e2]]) and define the normalized derivative operator $D$ ([[def-derivative]]) and the Serre derivative $\partial_k$ ([[def-serre-der]]) as the main tools to work with quasimodular forms.

![[def-derivative]]

Normalizing the derivative by $1/(2 \pi i)$ as in [[eq-derivative]] is standard in the theory of modular forms, since it makes the $q$-expansion coefficients nicer.

![[lemma-der-q-series]]

The most important example of quasimodular form is the weight 2 Eisenstein series $E_2$ ([[def-e2]]). Using it, we can define the *Serre derivative* of a quasimodular form.

![[def-serre-der]]

![[thm-serre-der-equiv-action]]

As a direct consequence of Theorem [[thm-serre-der-equiv-action]], we can check that the Serre derivative preserves the modularity of a modular form.

![[thm-serre-der-modularity]]

![[thm-ramanujan-formula]]

![[cor-logder-disc-e2]]

Similar argument allow us to compute (Serre) derivatives of $H_2, H_3, H_4$.

![[prop-theta-der]]

![[thm-serre-der-prod-rule]]

We also have the following useful theorem for proving positivity of quasimodular forms on the imaginary axis, which is [[ref-lee]].

![[thm-anti-serre-der-pos]]
