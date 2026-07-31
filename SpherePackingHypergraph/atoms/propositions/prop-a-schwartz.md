---
id: fa34f05af136
type: proposition
from: blueprint
lean:
  - MagicFunction.FourierEigenfunctions.a
formalized: true
---

# Proposition — prop:a-schwartz

## Statement

> [!proposition] prop:a-schwartz
> $a(x)$ is a [[def-schwartz-space|Schwartz function]].

## Proof

> [!note]- Proof (click to expand)
> By Theorem [[thm-smooth-fast-decay-schwartz]], it suffices to show that the function is smooth and decays faster than any polynomial. The smoothness follows from the “differentiation under the integral”, which is already formalized in `mathlib`. The decay follows from Lemmas [[lem-bound-i1-i3-i5]] and [[lem-bound-i2-i4-i6]], together with Lemma [[lem-integral-bound]].

**Uses**: [[cor-phi0-bound]], [[def-a-definition]].
