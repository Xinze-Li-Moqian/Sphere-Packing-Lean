---
type: notation
---

# Notation

Every term and symbol used in a Statement of this pool, with the card that
defines it. A row whose Card column is `—` is notation in use whose card
does not exist yet — a worklist, not an error.

**This table is read by the importer.** A row with a plain-text term and a
card links that term to that card everywhere it appears in the pool, which
is how a word like `density` gets linked at all: the automatic rule refuses
single words, because linking every occurrence of a common noun sends the
reader somewhere it did not mean. Here a person has decided, so it can.

Rows whose term is a formula are for reading only. Prose does not contain
formulas, and a link inside `$…$` renders as brackets.

**Written by hand.** The importer drafted it once and will not touch it again.

## Packings

| Notation | Meaning | Card |
|---|---|---|
| sphere packing | union of open balls of radius $r$ about a set of centres | [[spherepackingballs]] |
| separation radius | the $r$ with $\|x-y\| \ge r$ for distinct centres | [[spherepackingballs]] |
| density | $\limsup$ of the fraction of a large ball that is covered | [[spherepackingdensity]] |
| finite density | the same limit, when it exists | [[spherepackingfinitedensity]] |
| scaled packing | $\mathcal{P}(cX)$, with separation radius $cr$ | [[spherepackingscale]] |
| sphere packing constant | $\Delta_d$, the supremum of the density | [[spherepackingconstant]] |
| lattice | discrete additive subgroup spanning $\mathbb{R}^d$ | [[iszlattice]] |
| dual lattice | $\Lambda^* = \{ y : \langle x, y\rangle \in \mathbb{Z} \text{ for all } x \in \Lambda \}$ | [[def-dual-lattice]] |
| periodic packing | invariant under translation by a lattice | [[periodicspherepacking]] |
| periodic sphere packing constant | $\Delta_d^{\text{periodic}}$, the supremum over periodic packings | [[def-periodic-sphere-packing-constant]] |
| $E_8$ sphere packing | separation $\sqrt2$, centres $\Lambda_8$ — the optimal one in dimension eight | [[e8packing]] |
| $\Lambda_8$ | the $E_8$ lattice | [[e8packing]] |
| $\Delta_d$, $\Delta_P$ | the sphere packing constant; the density of $P$ | [[spherepackingconstant]] |

## Analysis

| Notation | Meaning | Card |
|---|---|---|
| Fourier transform | $\widehat f(y) = \int f(x)\, e^{-2\pi i \langle x, y\rangle}\,dx$ | [[def-fourier-transform]] |
| Schwartz function | smooth, with every derivative decaying faster than any power | [[def-schwartz-space]] |
| Schwartz space | the space of those | [[def-schwartz-space]] |
| $a_{\mathrm{rad}}$ | the radial function built from the $+1$ eigenfunction | [[def-a-definition]] |
| $b_{\mathrm{rad}}$ | the radial function built from the $-1$ eigenfunction | [[def-b-definition]] |

## Modular forms

| Notation | Meaning | Card |
|---|---|---|
| modular form | weight-$k$, level-$\Gamma$ function on $\mathbb{H}$, holomorphic at the cusps | [[def-mk]] |
| $M_k(\Gamma)$ | the space of them | [[def-mk]] |
| congruence subgroup | a subgroup containing some principal congruence subgroup | [[def-congruence-subgroup]] |
| principal congruence subgroup | $\Gamma(N)$: matrices congruent to the identity mod $N$ | [[def-level-n-princ-cong-subgp]] |
| $\Gamma(N)$ | the level $N$ principal congruence subgroup | [[def-level-n-princ-cong-subgp]] |
| $S$, $T$ | $z \mapsto -1/z$ and $z \mapsto z+1$, which generate $\Gamma_1$ | [[def-gamma-generators]] |
| automorphy factor | the $(cz+d)^k$ by which a form fails to be invariant | [[def-automorphy-factor]] |
| slash operator | the weight-$k$ action of $\gamma$ on a function | [[def-slash-operator]] |
| Eisenstein series | $E_k$, the weight-$k$ series summed over the lattice | [[def-ek]] |
| $E_2$ | the weight-two series — quasimodular, not modular | [[def-e2]] |
| discriminant form | $\Delta = (E_4^3 - E_6^2)/1728$ | [[def-disc-definition]] |
| Dedekind eta function | $\eta(z) = q^{1/24}\prod_{n\ge1} (1-q^n)$ | [[def-dedekind-eta]] |
| theta functions | the Thetanullwerte $\theta_{00}, \theta_{01}, \theta_{10}$ | [[def-th00-th01-th10]] |
| $\theta_{00}, \theta_{01}, \theta_{10}$ | the same three | [[def-th00-th01-th10]] |
| $H_2$, $H_3$, $H_4$ | the auxiliary forms built from them | [[def-h2-h3-h4]] |
| Serre derivative | $\partial_k = D - \tfrac{k}{12}E_2$, which preserves modularity | [[def-serre-der]] |
| $D$, $F'$ | the normalized derivative $\tfrac1{2\pi i}\tfrac{\mathrm{d}}{\mathrm{d}z}$ | [[def-derivative]] |
| $\varphi_4, \varphi_2, \varphi_0$ | the forms the $+1$ eigenfunction is assembled from | [[def-phi4-phi2-phi0]] |
| $\psi_I, \psi_T, \psi_S$ | their images under $I$, $T$ and $S$ | [[def-psii-psit-psis]] |
| $F$, $G$ | the two (quasi)modular forms of the $-1$ construction | [[def-fg-definition]] |
| $h$ | the auxiliary form of the $-1$ construction | [[def-h]] |

## Debt — in use, not yet defined here

| Notation | Meaning | Card |
|---|---|---|
| quasimodular form | modular but for a controlled $E_2$ term; assumed by the Serre derivative and by $F$, $G$ | — |
