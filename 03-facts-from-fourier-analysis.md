---
topic: sphere-packing-lean
type: topic
section: "3"
prose: narrative/03.md
---

# Facts from Fourier analysis

One identity carries the entire proof, and this section is here to state it and to make it legitimate.

## Poisson summation, and why it is the whole idea

For a lattice $\Lambda$ and a well-behaved $f$, $$\sum_{x \in \Lambda} f(x) \;=\; \frac{1}{\operatorname{covol}(\Lambda)}\sum_{y \in \Lambda^*} \hat f(y).$$

Read it as a translation. The left side is about a *packing* — where the points are, how close they get. The right side is about a *function* — the values of a Fourier transform. Poisson summation says these are the same number, so a fact one can arrange about the function becomes a fact one cannot otherwise reach about the arrangement.

That is the move the next section makes, and it is the only reason a question about stacking balls turns into a question about constructing a function.

## What has to be true for it to hold

The identity is false for arbitrary $f$: both sides can diverge, or converge to different things. The standard sufficient condition is that $f$ be **Schwartz** — smooth, with every derivative decaying faster than any polynomial. Schwartz functions are closed under the Fourier transform, which is what lets the identity be used in both directions.

The lemmas here are that toolkit: the Gaussian is its own transform (the prototype of everything in the last section), the transform is an automorphism of Schwartz space, and rapid decay makes the sums absolutely convergent so the rearrangements are allowed.

The reason to be careful is that the function the proof eventually builds is not given by a formula one can eyeball. It arrives as a contour integral, and showing it is Schwartz is real work — done in the last section, on the foundation laid here.


Recall the definition of a Fourier transform.

![[def-fourier-transform]]

The following computational result will be of use later on.

![[lemma-gaussian-fourier]]

Of great interest to us will be a specific family of functions, known as Schwartz Functions. The Fourier transform behaves particularly well when acting on Schwartz functions. We elaborate in the following subsections.


## On Schwartz Functions

![[def-schwartz-space]]

![[lemma-fourier-transform-is-automorphism]]

Another reason we are interested in Schwartz Functions is that they behave well under infinite sums. This will be useful to us when proving the Cohn-Elkies linear programming bound.


## On the Summability of Schwartz Functions


We begin by stating a general summability result over specific subsets of $\mathbb{R}^d$.

![[lemma-inv-power-summable]]

The decaying property of Schwartz functions means that they can be compared to the absolutely convergent power series above.

![[lemma-schwartz-summable]]

We end with a crucial result on Schwartz functions, the statement of which only makes sense because of the above result.

![[thm-poisson-summation-formula]]

While the Poisson Summation Formula over lattices can be stated in greater generality (and probably should be formalised as such in Mathlib due to the many applications it admits), we stick with Schwartz functions because that should be sufficient for our purposes.

Later, we will use Theorem [[thm-poisson-summation-formula]] to prove that the certain functions $a(x)$ and $b(x)$ that will be defined later are eigenfunctions of the Fourier transform. To apply the theorem, we need to show that these functions are Schwartz functions. We will do so by verifying the following sufficient condition.

![[thm-smooth-fast-decay-schwartz]]
