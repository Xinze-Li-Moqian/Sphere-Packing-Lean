---
topic: sphere-packing-lean
type: topic
section: "0"
date: 2026-07-31
---

# Sphere packings

How much of space can equal balls fill? Stack oranges and you get about $74\%$; that this is the best possible in three dimensions took from Kepler's guess in 1611 to Hales's proof in 1998, by way of an argument that ran to three hundred pages and a computer.

In dimension $8$ the answer is $\pi^4/384 \approx 25.37\%$, it is achieved by the $E_8$ lattice, and the proof is twenty-three pages long. That gap — three hundred pages in dimension three, twenty-three in dimension eight — is the first thing worth explaining, and it says something about which dimensions are hard rather than about who was cleverer.

## Why eight is easier than three

A packing problem has two halves. Finding a good arrangement is the easy half: somebody exhibits one and measures it. Proving nothing beats it is the hard half, because the space of arrangements is enormous and mostly disordered — there is no reason a densest packing should be a lattice, and in most dimensions it is believed not to be.

What makes dimension $8$ tractable is that $E_8$ is *rigid* in a way no three-dimensional arrangement is. It is not merely a good packing; it sits at a coincidence where a general upper bound, applied to it, gives back exactly its own density. The whole proof consists of showing that this coincidence is real rather than numerical.

## What has to be defined first

The mathematics below is unglamorous and unavoidable: to say "no packing is denser" one must first say what a packing is, what its density is, and why that number exists at all.

The subtlety is the last one. A packing is an infinite object, so its density has to be a limit — the fraction of a large ball that is covered, as the ball grows. That limit need not exist for an arbitrary arrangement, which is why the definition takes a limit superior and why the sections that follow work to show the sloppiness does no harm.


The Sphere Packing problem is a classic optimisation problem with widespread applications that go well beyond mathematics. The task is to determine the “densest” possible arrangement of spheres in a given space. It remains unsolved in all but finitely many dimensions.

It was famously determined, in [[ref-via2017]], that the optimal arrangement in $\mathbb{R}^8$ is given by the $E_8$ lattice. The result is strongly dependent on the Cohn-Elkies linear programming bound (Theorem 3.1 in [[ref-elkiescohn]]), which, if a $\mathbb{R}^d \to \mathbb{R}$ function satisfying certain conditions exists, bounds the optimal density of sphere packings in $\mathbb{R}^d$ in terms of it. The proof in [[ref-via2017]] uses the theory of modular forms to construct a function that can be used to bound the density of all sphere packings in $\mathbb{R}^8$ above by the density of the $E_8$ lattice packing. This then allows us to conclude that no packing in $\mathbb{R}^8$ can be denser than the $E_8$ lattice packing.


## The Setup


This subsection gives an overview for the setup of the problem, both informally and in Lean. Throughout this blueprint, $\mathbb{R}^d$ will denote the Euclidean vector space equipped with distance $\|\cdot\|$ and Lebesgue measure $\mathrm{Vol}(\cdot)$. For any $x\in\mathbb{R}^d$ and $r\in\mathbb{R}_{>0}$, we denote by $B_d(x,r)$ the open ball in $\mathbb{R}^d$ with center $x$ and radius $r$. While we will give a more formal definition of a sphere packing below (and in Lean), the underlying idea is that it is a union of balls of equal radius centred at points that are far enough from each other that the balls do not overlap.

Arguably the most important definition in this subsection is that of *packing density*, which measures which portion of $d$-dimensional Euclidean space is covered by a given sphere packing. Taking the supremum over all packings gives what we refer to as the *sphere packing constant*, which is the quantity we are interested in optimising.

![[spherepackingballs]]

![[spherepacking]]

We now define a notion of density for bounded regions of space by considering the density inside balls of finite radius.

![[spherepackingfinitedensity]]

As intuitive as it seems to take the density of a packing to be the limit of the finite densities as the radius of the ball goes to infinity, it is not immediately clear that this limit exists. Therefore, we define the density of a sphere packing as a limit superior instead.

![[spherepackingdensity]]

We may now define the sphere packing constant, the quantity that the sphere packing problem requires us to compute.

![[spherepackingconstant]]

## Scaling Sphere Packings


Given that the problem involves the *arrangement* of balls in space, it is intuitive not to worry about the radius of the balls (so long as they are all equal to each other). However, Definition [[spherepackingballs]] involves a choice of separation radius. In principle, we would want two sphere packing configurations that differ only in separation radii to ‘encode the same information’. In this brief subsection, we will describe how to change the separation radius of a sphere packing by *scaling* the packing by a positive real number and prove that this does not affect its density. This will give us the freedom to choose any separation radius we like when attempting to define the optimal sphere packing in $\mathbb{R}^d$.

![[spherepackingscale]]

![[spherepackingscale-finitedensity]]

![[spherepackingscale-density]]

Therefore, as expected, we do not need to worry about the separation radius when constructing sphere packings. This will be useful when we attempt to construct the optimal sphere packing in $\mathbb{R}^8$---and even more so when attempting to *formalise* this construction---because the underlying structure of the packing is given by a set known as the $E_8$ lattice, which has separation radius $\sqrt{2}$.

We can also use Lemma [[spherepackingscale-density]] to simplify the computation of the sphere packing constant by taking the supremum not over *all* sphere packings but only over those with density $1$.

![[spherepackingconstant-eq-constant-normalized]]

## Lattices and Periodic packings


We begin by defining what a lattice is in Euclidean space.

![[iszlattice]]

There is also a corresponding dual notion, which will become relevant when we start doing Fourier analysis on functions over lattices.

![[def-dual-lattice]]

We can now define periodic sphere packings.

![[periodicspherepacking]]

There is a natural definition of density for periodic sphere packings, namely the “local” density of balls in a fundamental domain. However, *a priori* the density of sphere packing above need not to coincide with this alternative definition. In [[theorem-psp-density]], we will prove that this is the case.

Now that we have simplified the process of computing the packing densities of specific packings, we can simplify that of computing the sphere packing constant. It turns out that once again, periodicity is key.

![[def-periodic-sphere-packing-constant]]

![[thm-periodic-packing-optimal]]

Thus, one can show a sphere packing to be optimal by showing its density to be equal to the *periodic* sphere packing constant instead of the regular sphere packing constant. The determination of the periodic constant is easier than that of the general constant, as we shall see when investigating the Linear Programming bounds derived by Cohn and Elkies in [[ref-elkiescohn]].

## Main Result


With the terminologies above, we can state the main theorem of this project.

![[theorem-ce-main]]

![[corollary-upper-bound-e8]]

![[maintheorem]]
