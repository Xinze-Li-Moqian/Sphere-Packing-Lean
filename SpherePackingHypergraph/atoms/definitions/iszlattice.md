---
id: a928d37bc70f
type: definition
from: blueprint
lean:
  - IsZLattice
formalized: true
---

# Definition — IsZLattice

## Statement

> [!definition] IsZLattice
> We say that an additive subgroup $\Lambda \leq \mathbb{R}^d$ is a *lattice* if it is discrete and its $\mathbb{R}$-span contains all the elements of $\mathbb{R}^d$.

**Used by**: [[def-dual-lattice]], [[e8-matrix]], [[e8-set]], [[instdiscretee8lattice]].

## Notes

> [!note]- Notes (click to expand)
> - The condition is two-sided: discreteness rules out dense subgroups like $\mathbb{Z} + \sqrt2\,\mathbb{Z} \subset \mathbb{R}$, and full $\mathbb{R}$-span rules out lattices of a lower-dimensional subspace.
> - [[e8-set|$\Lambda_8$]] is the lattice this development is about, and [[e8-defs-equivalent]] identifies it with the $\mathbb{Z}$-span of [[e8-matrix|eight explicit vectors]].
> - Every lattice has a [[def-dual-lattice|dual]], and it is self-duality that makes Poisson summation say something about $\Lambda_8$ rather than about two different sets of points.
> - A packing whose centres are invariant under a lattice is [[periodicspherepacking|periodic]]; a lattice packing is the special case where the centres *are* the lattice.
