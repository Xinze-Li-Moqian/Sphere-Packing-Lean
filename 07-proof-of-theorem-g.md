---
topic: sphere-packing-lean
type: topic
section: "7"
prose: narrative/07.md
---

# Proof of Theorem g

The construction is finished; what remains is to check that the function it produced actually has the signs the Cohn–Elkies bound demands.

That sounds like an afterthought and is not. The bound needs $f \le 0$ beyond the unit ball and $\hat f \ge 0$ everywhere — two inequalities that have to hold at every point of $\mathbb{R}^8$, for a function defined by a contour integral. There is no evaluating it and looking.

## Turning an inequality into an identity

The way through is to stop reasoning about the function and reason about the modular forms it was built from. Written in $q = e^{2\pi i z}$, each form is a power series with explicit coefficients, and a statement about the sign of the function becomes a statement about those coefficients.

Some of them are settled by writing the form as a product of things already known to be positive. The harder ones are settled by a differential equation: showing a quantity is monotone in $q$, and then checking its limit at one endpoint. Positivity at every point follows from positivity at a boundary plus a derivative that never changes sign.

## What is proved

The two inequalities, and with them the theorem. Cohn and Elkies gave the bound in 2003 and could not produce a function; the function is this one, and the number it yields is exactly the density of $E_8$.


Our proof of the Theorem [[thm-g]] relies on the following two inequalities for modular objects.

![[prop-ineqa]]

![[prop-ineqb]]

Here we formalize the proof of the inequalities by Lee [[ref-lee]]. First, we can rewrite the inequality in [[prop-ineqa]] as follows.

![[def-fg-definition]]

![[lemma-f-g-phi-psi-identities]]

![[lemma-ineqabnew-equiv]]

Now, the first inequality [[eq-ineqanew]] follows from the positivity of each $F(it)$ and $G(it)$.

![[lemma-f-g-pos]]

![[cor-ineqanew]]

To prove the second inequality [[eq-ineqbnew]], we need some identities satisfied by $F$ and $G$.

![[lemma-fg-de]]

![[cor-mlde-pos]]

The second inequality [[eq-ineqbnew]] follows from the following two observations.
Since $G(it) > 0$ for all $t > 0$, we can define the quotient
$$
Q(t) := \frac{F(it)}{G(it)}
$$
as a function on $(0, \infty)$.

![[lemma-qlim]]

![[lemma-log-der-inf]]

![[prop-qdec]]

![[cor-ineqbnew]]

Finally, we are ready to prove Theorem [[thm-g]].

![[thm-g1]]
