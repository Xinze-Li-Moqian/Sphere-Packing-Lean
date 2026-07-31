---
id: ff4f79a46d91
type: definition
from: blueprint
lean:
  - ModularGroup.S
  - ModularGroup.T
  - α
  - β
formalized: true
---

# Definition — def:Gamma-generators

## Statement

> [!definition] def:Gamma-generators
> Define the matrices
> 
> $$S = \begin{pmatrix} 0 & -1 \\ 1 & 0 \end{pmatrix} \in \Gamma_1,
> T = \begin{pmatrix} 1 & 1 \\ 0 & 1 \end{pmatrix} \in \Gamma_1,
> \alpha = \begin{pmatrix} 1 & 2 \\ 0 & 1 \end{pmatrix} \in \Gamma_2 \subset \Gamma_1,
> \beta = \begin{pmatrix} 1 & 0 \\ 2 & 1 \end{pmatrix} \in \Gamma_2 \subset \Gamma_1.$$
> 
> It is easily verifiable that $\alpha = T^2$ and $\beta = -S\alpha^{-1}S = -ST^{-2}S$.

**Uses**: [[def-level-n-princ-cong-subgp]].
