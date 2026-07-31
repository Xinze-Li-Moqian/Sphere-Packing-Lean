---
topic: sphere-packing-lean
type: topic
section: "1"
prose: narrative/01.md
---

# Density of packings

The definition of density takes a limit superior over growing balls, which is an admission that the limit might not exist. This section removes the admission for the packings the argument actually needs.

## Why periodic packings are enough

The optimum is a supremum over all packings, and most packings have no structure whatever. The reduction here is that nothing is lost by looking only at **periodic** ones — packings invariant under a lattice, so that finitely many balls repeat forever.

The idea is a cut-and-repeat: take any packing, cut out a large cube, and tile space with copies of it. Balls near the cut are damaged, but the damage lives on the surface of the cube while the density lives in its volume — and surface grows like $R^{d-1}$ where volume grows like $R^d$. Enlarging the cube drives the loss to nothing.

That is the whole content, and it is why the estimates below are about counting lattice points in a ball and comparing volumes of concentric balls. They are the bookkeeping for "the boundary does not matter".

## What this buys

Everything after this section may assume a lattice is present. That matters more than it sounds: the bound in the next sections runs on Poisson summation, and Poisson summation needs a lattice to sum over. Without this reduction the main tool would not apply to the problem at all.


The definition of density given in [[00-sphere-packings]] is inconvenient to work with, especially when our packing is a structured one, such as a periodic/lattice packing. This section fixes this problem.

Note that some of the proofs in this section have only been sketched. The finer details are formalised in Lean.

Observe that the finite density evaluated at some $R > 0$ measures the density of sphere packings within a bounded, open ball of radius $R$. As one might expect, there is a relationship between the finite density and the number of centers in the ball of radius $R$.

![[lemma-sp-finite-density-bound]]

Suppose further that $X$ is a periodic packing w.r.t. the lattice $\Lambda \subseteq \mathbb{R}^d$. Let $\mathcal{D}$ be a (bounded) fundamental region of $\Lambda$, say the parallelopiped $[0, 1]^n\Lambda$, and let $L$ be the bound on the norm of vectors in $\mathcal{D}$, i.e. a number satisfying $\forall x \in \mathcal{D}, \|x\| \leq L$.

![[lemma-lattice-points-bound]]

To link [[lemma-sp-finite-density-bound]] and [[lemma-lattice-points-bound]], we need a lemma relating $|\Lambda \cap \mathcal{B}|$ with $|X \cap \mathcal{B}|$, which is what the following lemma does:

![[lemma-periodic-points-bounds]]

When we combine the inequalities above, we need one additional computational lemma.

![[lemma-volume-ball-ratio-limit]]

Finally, we can relate the density of a periodic sphere packing to the natural definition of density given by any of its fundamental domain:

![[theorem-psp-density]]
