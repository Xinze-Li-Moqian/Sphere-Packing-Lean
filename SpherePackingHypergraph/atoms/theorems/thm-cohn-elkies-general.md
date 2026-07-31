---
id: 5a34442b4911
type: theorem
lean:
  - LinearProgrammingBound
formalized: true
---

# Theorem — Cohn–Elkies [[ref-elkiescohn]]

## Statement

> [!theorem] Cohn–Elkies [[ref-elkiescohn]]
> Let $f:\mathbb{R}^d\to\mathbb{R}$ be a Schwartz function that is not identically zero and satisfies [[eq-cohn-elkies-condition-1]] and [[eq-cohn-elkies-condition-2]]. Then the density of any $\Lambda$-periodic sphere packing is bounded above by $$\frac{f(0)}{\widehat{f}(0)}\cdot \mathrm{vol}(B_d(0,1/2)).$$

## Proof

> [!note]- Proof (click to expand)
> The result follows immediately from Theorem [[thm-periodic-packing-optimal]] and [[thm-cohn-elkies-periodic]].
