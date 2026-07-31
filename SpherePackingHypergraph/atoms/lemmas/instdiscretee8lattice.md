---
id: 8517c40c36c8
type: lemma
lean:
  - instDiscreteE8Lattice
formalized: true
---

# Lemma — instDiscreteE8Lattice

## Statement

> [!lemma] instDiscreteE8Lattice
> $c\Lambda_8$ is discrete, i.e. that the subspace topology induced by its inclusion into $\mathbb{R}^8$ is the discrete topology.

## Proof

> [!note]- Proof (click to expand)
> Since $\Lambda_8$ is a topological group and $+$ is continuous, it suffices to prove that $\{0\}$ is open in $\Lambda_8$. This follows from the fact that there is an open ball $\mathcal{B}(\sqrt{2}) \subseteq \mathbb{R}^8$ around it containing no other lattice points, since the shortest nonzero vector has norm $\sqrt{2}$.
