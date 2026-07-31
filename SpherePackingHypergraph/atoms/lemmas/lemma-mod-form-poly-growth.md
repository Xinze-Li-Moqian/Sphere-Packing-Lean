---
id: 0597154359a8
type: lemma
from: blueprint
formalized: true
---

# Lemma — lemma:mod_form_poly_growth

## Statement

> [!lemma] lemma:mod_form_poly_growth
> : Let $\Gamma$ be a finite index subgroup of $\mathrm{SL}_2(\mathbb{Z})$ and $f \in \mathcal{M}_k(\Gamma)$ be a [[def-mk|modular form]] of weight $k$. Then the Fourier coefficients $a_n(f)$ has a polynomial growth, i.e. $|a_n(f)| = O(n^k)$.

## Proof

> [!note]- Proof (click to expand)
> Note that the assumption on the polynomial growth holds when $f$ is a holomorphic modular form, where the proof can be found in [[ref-serre73]] for the case of level 1 modular forms. This has been done in Lean 4 by David Loeffler.
