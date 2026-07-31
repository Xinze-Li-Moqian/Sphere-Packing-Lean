---
id: 5aaf2c22cfd5
type: lemma
from: blueprint
lean:
  - instIsZLatticeE8Lattice
formalized: true
---

# Lemma — instLatticeE8

## Statement

> [!lemma] instLatticeE8
> $c\Lambda_8$ is a $\mathbb{Z}$-[[iszlattice|lattice]], i.e. it is discrete and spans $\mathbb{R}^8$ over $\mathbb{R}$.

## Proof

> [!note]- Proof (click to expand)
> The first part is by [[instdiscretee8lattice]], and the second part follows from that $\mathcal{B}_8$ is a basis ([[e8-is-basis]]) and hence linearly independent over $\mathbb{R}$.
