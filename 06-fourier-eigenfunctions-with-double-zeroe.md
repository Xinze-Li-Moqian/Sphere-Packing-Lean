---
topic: sphere-packing-lean
type: topic
section: "6"
prose: narrative/06.md
---

# Fourier eigenfunctions with double zeroes at lattice points

This is the construction. Everything before it was setting the specification; this section produces a function meeting it, and with that the theorem is proved.

## Splitting the problem in two

The requirement couples $f$ to $\hat f$, and coupled requirements are hard. The first move decouples them.

The Fourier transform squares to the identity on radial functions, so it has eigenvalues $+1$ and $-1$, and every radial function splits as a sum of an eigenfunction of each. Build the two pieces separately: a function $a$ with $\hat a = a$, and a function $b$ with $\hat b = -b$. For an eigenfunction the condition "$f$ and $\hat f$ both vanish at $\sqrt{2n}$" collapses to a condition on one function.

Both halves are then built the same way, which is why this section reads twice through with $\varphi$ replaced by $\psi$ and $a$ by $b$.

## How each half is built

Integrate a modular form against the Gaussian family: $$a(x) \;=\; \int \varphi(z)\, e^{\pi i \|x\|^2 z}\, dz$$ along a contour in the upper half plane.

Three things then happen, and each is a section of the mathematics below.

**The eigenfunction property comes from modularity.** Applying the Fourier
transform sends the Gaussian's parameter $z$ to $-1/z$; deforming the contour
back and using how $\varphi$ transforms under $z \mapsto -1/z$ returns the
same integral, up to the sign that decides which eigenfunction it is. This is
the step the whole apparatus of the previous section exists to license.

**The double zeros come from the $q$-expansion.** Written in $q = e^{2\pi i z}$,
the integral picks out where the expansion has integer exponents, and the
radii at which the result vanishes are exactly $\sqrt{2n}$ — the lengths
$E_8$ uses. The order of vanishing is two because the expansion begins one
term later than one might expect.

**Being Schwartz is work.** The integrand grows badly near the boundary of the
contour, and the bounds below — on $\varphi$, on $\psi$, on the six integrals
each is broken into — exist to show that the integral converges, defines a
smooth function, and decays fast enough. This is the least beautiful part and
the largest.

## Assembling

With $a$ and $b$ in hand, $f$ and $g$ are explicit combinations. What is left is the sign conditions — $f \le 0$ outside the unit ball, $\hat f \ge 0$ everywhere — and these are inequalities about specific modular forms, proved by writing the forms in terms of $q$ and showing the coefficients behave.

The final statement records that the resulting function makes the Cohn–Elkies bound equal to the density of $E_8$. Combined with the bound itself, from four sections ago, that is the theorem: no packing in $\mathbb{R}^8$ is denser than $E_8$.


In this section we construct two radial Schwartz functions $a,b:\mathbb{R}^8\to i\mathbb{R}$ such that
$$
\begin{aligned}\mathcal{F}(a)&=a\\
\mathcal{F}(b)&=-b
\end{aligned}
$$
which double zeroes at all $\Lambda_8$-vectors of length greater than $\sqrt{2}$. Recall that each vector of $\Lambda_8$ has length $\sqrt{2n}$ for some $n\in\mathbb{N}_{\geq 0}$.
We define $a$ and $b$ so that their values are purely imaginary because this simplifies some of our computations.
We will show in Section [[07-proof-of-theorem-g]] that an appropriate linear combination of functions $a$ and $b$ satisfies conditions [[eq-g1]]--[[eq-g3]].

Both of the functions will be defined via certain integrals of (quasi)modular forms. Then the eigenfunction property mainly follows from the Poisson summation formula (Theorem [[thm-poisson-summation-formula]]) and the transformation laws of (quasi)modular forms. To apply Theorem [[thm-poisson-summation-formula]], we will show that $a(x)$ and $b(x)$ are Schwartz functions, and this can be proved by verifying fast decay of the integrals.

First, we will define function $a$. To this end we consider the following functions:

![[def-phi4-phi2-phi0]]

The function $\phi_0(z)$ is not modular; however, it satisfies the following transformation rules:

![[lemma-phi0-transform]]

For our formalization, we choose rectangular contours for the first and the second integral, and write it as follows.

![[def-a-definition]]

In the original paper, the integrals $I_1$ and $I_2$ are combined, as well as $I_3$ and $I_4$. We choose to write them separately to simplify the formalization.

Now we prove that $a$ satisfies condition [[eq-a-fourier]]. The following lemma will be used to prove Schwartzness of $a$ and $b$.

![[lemma-mod-div-disc-bound]]

When $f(z)$ is a (quasi)modular form, we can take $k$ to be the weight of $f$.

As corollaries, we have the following bound for $\phi_0$, $\phi_{-2}$, and $\phi_{-4}$.

![[cor-phi0-bound]]

![[cor-phi2-bound]]

![[cor-phi4-bound]]

Note that we can take the constants $C_0$, $C_{-2}$, and $C_{-4}$ as
$$
\begin{aligned}
C_0 &= 9 \cdot 240^2 \cdot e^{\pi} \cdot \frac{E_4'(i/2)^{2}}{\Delta(i/2)} \notag \\
C_{-2} &= 3 \cdot \frac{E_4(i/2) E_4'(i/2)}{\Delta(i/2)} \notag \\
C_{-4} &= e^{-\pi} \cdot \frac{E_4(i/2)^{2}}{\Delta(i/2)}. \notag
\end{aligned}
$$

![[lem-integral-bound]]

![[lem-bound-i1-i3-i5]]

Combined with Lemma [[lem-integral-bound]], this shows that the integrals $I_1$, $I_3$, and $I_5$ decay faster than any polynomial as $r \to \infty$. For the integrals $I_2$, $I_4$, and $I_6$, it is easier to see this since the contours are not touching the real axis.

![[lem-bound-i2-i4-i6]]

Combining these, one can show that $a$ is a Schwartz function.

![[prop-a-schwartz]]

![[prop-a-fourier]]

Next, we check that $a$ has double zeroes at all $\Lambda_8$-lattice points of length greater then $\sqrt{2}$. Using [[eq-phi0-bound]], [[eq-phi2-bound]], and [[eq-phi4-bound]], we can control the behavior of $\phi_0$ near $0$ and $i\infty$.

![[cor-phi0-near-0-infty]]

![[prop-a-double-zeros]]

Finally, we find another convenient integral representation for $a$ and compute values of $a(r)$ at $r=0$ and $r=\sqrt{2}$.

![[prop-a-another-integral]]

From the identity [[eq-a-another-integral]] we see that the values $a(r)$ are in $i\mathbb{R}$ for all $r\in\mathbb{R}_{\geq0}$.

![[prop-a0]]

Now we construct function $b$. To this end we consider the function

![[def-h]]

It is easy to see that $h\in M^!_{-2}(\Gamma_0(2))$. Indeed, first we check that $h|_{-2}\gamma=h$
for all $\gamma\in\Gamma_0(2)$. Since the group $\Gamma_0(2)$ is generated by elements
$\left(\begin{smallmatrix}1&0\\2&1\end{smallmatrix}\right)$ and $\left(\begin{smallmatrix}1&1\\0&1\end{smallmatrix}\right)$
it suffices to check that $h$ is invariant under their action. This follows immediately
from [[eq-h2-transform-s]]--[[eq-h4-transform-s]] and [[def-h]]. Next we analyze the poles of $h$.
It is known [[ref-mumford]] that $\theta_{10}$ has no zeros in the upper-half plane and hence $h$ has poles only at the cusps.
At the cusp $i\infty$ this modular form has the Fourier expansion

$$
h(z)\,=\,q^{-1} + 16 - 132 q + 640 q^2 - 2550 q^3+O(q^4).
$$

Let $I=\left(\begin{smallmatrix}1&0\\0&1\end{smallmatrix}\right)$,
$T=\left(\begin{smallmatrix}1&1\\0&1\end{smallmatrix}\right)$, and
$S=\left(\begin{smallmatrix}0&-1\\1&0\end{smallmatrix}\right)$ be elements of $\Gamma_1$.

![[def-psii-psit-psis]]

![[lemma-psi-new]]

![[lemma-psii-psit-psis-fourier]]

Now, we are ready to define function $b$. Again, the definition here is slightly different from that in [[ref-via2017]], where all the contours are chosen to be the straight lines.

![[def-b-definition]]

Now we prove that $b$ is a Schwartz function and satisfies condition [[eq-b-fourier]]. As in the case of $a(x)$, we start with the following exponential bound of $\psi_S(z)$ and $\psi_I(z)$.

![[lemma-psi-bound]]

![[lemma-bound-j1-j3-j5]]

![[lemma-bound-j2-j4-j6]]

Combining Lemmas [[lemma-bound-j1-j3-j5]], [[lemma-bound-j2-j4-j6]], and Theorem [[thm-smooth-fast-decay-schwartz]], we can prove that $b(x)$ is a Schwartz function.

![[prop-b-schwartz]]

![[prop-b-fourier]]

Now we regard the radial function $b$ as a function on $\mathbb{R}_{\geq0}$. We check that $b$ has double roots at $\Lambda_8$-points.

![[cor-psii-near-0-infty]]

![[prop-b-double-zeros]]

At the end of this section we find another integral representation of $b(r)$ for $r\in\mathbb{R}_{\geq0}$ and compute special values of $b$.

![[prop-b-another-integral]]

We see from [[eq-b-another-integral]] that $b(r)\in i\mathbb{R}$ far all $r\in\mathbb{R}_\geq{0}$. Another immediate corollary of this proposition is

![[prop-b0]]
