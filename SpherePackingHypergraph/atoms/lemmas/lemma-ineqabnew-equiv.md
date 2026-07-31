---
id: 0c22586dabf8
type: lemma
from: blueprint
---

# Lemma — lemma:ineqABnew-equiv

## Statement

> [!lemma] lemma:ineqABnew-equiv
> Inequality [[eq-ineqa]] and [[eq-ineqb]] are equivalent to
> $$
> \begin{aligned}
> F(it) + \frac{18}{\pi^2} G(it) > 0  \\
> F(it) - \frac{18}{\pi^2} G(it) > 0 
> \end{aligned}
> $$
> respectively.

## Proof

> [!note]- Proof (click to expand)
> By [[eq-psis-define]],
> $$
> \psi_I(it) = (\psi_S|_{-2}S)(it) = (it)^{2}\psi_S\left(-\frac{1}{it}\right) = -t^2 \psi_S\left(\frac{i}{t}\right).
> $$
> Combined with Lemma [[lemma-f-g-phi-psi-identities]] we can rewrite [[eq-ineqa]] as
> $$
> A(t) = -t^2 \phi_0\left(\frac{i}{t}\right) + \frac{36}{\pi^2} \psi_S\left(\frac{i}{t}\right) < 0 \Leftrightarrow \frac{F(it)}{\Delta(it)} + \frac{18}{\pi^2} \frac{G(it)}{\Delta(it)} > 0
> $$
> for $t > 0$, which is equivalent to [[eq-ineqanew]] by Corollary [[cor-disc-pos]].
> Equivalences of [[eq-ineqb]] and [[eq-ineqbnew]] follows similarly; just change the sign.

**Uses**: [[cor-disc-pos]], [[def-psii-psit-psis]], [[lemma-f-g-phi-psi-identities]].
