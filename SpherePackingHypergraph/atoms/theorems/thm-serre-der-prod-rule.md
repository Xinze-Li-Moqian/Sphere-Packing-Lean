---
id: 43d5f1374a54
type: theorem
lean:
  - serre_D_mul
formalized: true
---

# Theorem — thm:serre-der-prod-rule

## Statement

> [!theorem] thm:serre-der-prod-rule
> The [[def-serre-der|Serre derivative]] satisfies the following product rule: for any quasimodular forms $F$ and $G$,
> $$
> \partial_{w_1 + w_2} (FG) = (\partial_{w_1}F)G + F (\partial_{w_2}G).
> $$

## Proof

> [!note]- Proof (click to expand)
> It follows from the definition:
> $$
> \begin{aligned}
> \partial_{w_1 + w_2} (FG) &= (FG)' - \frac{w_1 + w_2}{12} E_2 (FG) \\
> &= F'G + FG' - \frac{w_1 + w_2}{12} E_2(FG) \\
> &= \left(F' - \frac{w_1}{12}E_2 F\right)G + F \left(G' - \frac{w_2}{12}E_2 G\right) \\
> &= (\partial_{w_1}F)G + F(\partial_{w_2}G).
> \end{aligned}
> $$
