---
id: b8d6c8d37282
type: lemma
from: blueprint
lean:
  - MLDE_F
  - MLDE_G
formalized: true
---

# Lemma — lemma:FG-de

## Statement

> [!lemma] lemma:FG-de
> $F$ and $G$ satisfy the following differential equations:
> $$
> \begin{aligned}
> \partial_{12}\partial_{10} F - \frac{5}{6} E_{4} F &= 7200 \Delta (-E_{2}')  \\
> \partial_{12}\partial_{10} G - \frac{5}{6} E_{4} G &= -640 \Delta H_{2} 
> \end{aligned}
> $$

**In terms of**: [[def-disc-definition]], [[def-ek]], [[def-e2]], [[def-h2-h3-h4]].

## Proof

> [!note]- Proof (click to expand)
> Both can be shown by direct computations.
> By Ramanujan's identities (Theorem [[thm-ramanujan-formula]]) and the product rule of [[def-serre-der|Serre derivatives]] (Theorem [[thm-serre-der-prod-rule]]), we have
> $$
> \begin{aligned}
> \partial_{5} (E_2 E_4 - E_6) &= (E_2 E_4 - E_6)' - \frac{5}{12} E_2 (E_2 E_4 - E_6) \\
> &= \frac{E_2^2 - E_4}{12} \cdot E_4 + E_2 \cdot \frac{E_2 E_4 - E_6}{3} - \frac{E_2 E_6 - E_4^2}{2} - \frac{5}{12}E_2 (E_2 E_4 - E_6) \\
> &= -\frac{5}{12} (E_2 E_6 - E_4^2)  \\
> \partial_{7} (E_2 E_6 - E_4^2) &= (E_2 E_6 - E_4^2)' - \frac{7}{12} E_2 (E_2 E_6 - E_4^2) \\
> &= \frac{E_2^2 - E_4}{12} \cdot E_6 + E_2 \cdot \frac{E_2 E_6 - E_4^2}{2} - 2 E_4 \cdot \frac{E_2 E_4 - E_6}{3} - \frac{7}{12} E_2 (E_2 E_6 - E_4^2) \\
> &= -\frac{7}{12} E_4 (E_2 E_4 - E_6) 
> \end{aligned}
> $$
> and using these we can compute
> $$
> \begin{aligned}
> \partial_{10} F &= \partial_{10} (E_2 E_4 - E_6)^2 \\
> &= 2 (E_2 E_4 - E_6) \partial_{5} (E_2 E_4 - E_6) \\
> &= -\frac{6}{5} (E_2 E_4 - E_6) (E_2 E_6 - E_4^2), \\
> \partial_{12}\partial_{10} F &= -\frac{5}{6} \partial_{12} ((E_2 E_4 - E_6) (E_2 E_6 - E_4)) \\
> &= -\frac{5}{6} (\partial_{5}(E_2 E_4 - E_6)) (E_2 E_6 - E_4^2) - \frac{5}{6} (E_2 E_4 - E_6) (\partial_{7} (E_2 E_6 - E_4)) \\
> &= \frac{25}{72} (E_2 E_6 - E_4^2)^2 + \frac{35}{72} E_4 (E_2 E_4 - E_6)^2, \\
> \partial_{12}\partial_{10}F - \frac{5}{6} E_4 F &= \frac{25}{72}(E_2 E_6 - E_4^2)^2 + \frac{35}{72} E_4 (E_2 E_4 - E_6)^2 - \frac{5}{6} E_4 (E_2 E_4 - E_6)^2 \\
> &= \frac{25}{72} ((E_2 E_6 - E_4^2)^2 - E_4 (E_2 E_4 - E_6)^2) \\
> &= \frac{25}{72} (- E_2^2 E_4^3 + E_2^2 E_6^2 + E_4^4 - E_4 E_6^3) \\
> &= -\frac{25}{72} (E_4^3 - E_6^2) (E_2^2 - E_4) \\
> &= 7200 \cdot \frac{E_4^3 - E_6^2}{1728} \cdot \frac{-E_2^2 + E_4}{12}\\
> &= 7200 \Delta (-E_2')
> \end{aligned}
> $$
> which proves [[eq-ddf]].
> Similarly, [[eq-ddg]] can be proved using Proposition [[prop-theta-der]] and Lemma [[lemma-lv1-lv2-identities]].

**Uses**: [[lemma-lv1-lv2-identities]], [[prop-theta-der]], [[thm-ramanujan-formula]], [[thm-serre-der-prod-rule]].
