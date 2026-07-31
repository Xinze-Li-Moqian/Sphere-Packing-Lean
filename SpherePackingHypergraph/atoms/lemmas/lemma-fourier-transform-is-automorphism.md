---
id: 97c2182a4de4
type: lemma
lean:
  - SchwartzMap.fourierTransformCLM
formalized: true
---

# Lemma — lemma:Fourier-transform-is-automorphism

## Statement

> [!lemma] lemma:Fourier-transform-is-automorphism
> The [[def-fourier-transform|Fourier transform]] is a continuous, linear automorphism of the space of [[def-schwartz-space|Schwartz functions]].

## Proof

> [!note]- Proof (click to expand)
> We do not elaborate here as the result already exists in Mathlib. We do, however, mention that the Lean implementation *defines* a continuous linear equivalence on the [[def-schwartz-space|Schwartz space]] *using* the Fourier transform (see `SchwartzMap.fourierTransformCLM`). The ‘proof’ that for any Schwartz function $f$, its Fourier transform and its image under this continuous linear equivalence are, indeed, the same $\mathbb{R}^d \to \mathbb{R}$ function, is stated in Mathlib solely for the purpose of `rw` and `simp` tactics, and is proven simply by `rfl`.
