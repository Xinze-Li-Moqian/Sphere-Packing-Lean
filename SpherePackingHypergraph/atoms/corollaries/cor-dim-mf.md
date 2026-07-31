---
id: 0121928434d9
type: corollary
formalized: true
---

# Corollary — cor:dim-mf

## Statement

> [!corollary] cor:dim-mf
> We have
> $$
> \begin{aligned}
> \dim M_2(\mathrm{SL}_{2}(\mathbb{Z})) &= 0,  \\
> \dim M_4(\mathrm{SL}_{2}(\mathbb{Z})) &= 1,  \\
> \dim M_6(\mathrm{SL}_{2}(\mathbb{Z})) &= 1,  \\
> \dim M_8(\mathrm{SL}_{2}(\mathbb{Z})) &= 1,  \\
> \dim S_4(\mathrm{SL}_{2}(\mathbb{Z})) &= 0,  \\
> \dim S_6(\mathrm{SL}_{2}(\mathbb{Z})) &= 0,  \\
> \dim S_8(\mathrm{SL}_{2}(\mathbb{Z})) &= 0. 
> \end{aligned}
> $$

**In terms of**: [[def-cusp-form]].

## Proof

> [!note]- Proof (click to expand)
> Each line is [[thm-lvl1-dims]] evaluated at one even weight: $\dim M_k(\Gamma_1)=\lfloor k/12\rfloor$ when $k\equiv 2 \pmod{12}$, and $\lfloor k/12\rfloor+1$ otherwise.
>
> So $\dim M_2=\lfloor 2/12\rfloor=0$, while for $k=4,6,8,10$ the formula gives $0+1=1$ — each space is spanned by its [[def-ek|Eisenstein series]] — and at $k=12$ it gives $1+1=2$, the new dimension being the first [[def-cusp-form|cusp form]], [[def-disc-definition|$\Delta$]].
>
> The cuspidal statements follow by subtracting one for the Eisenstein series: $\dim S_k=\dim M_k-1$ for even $k\ge 4$, so $S_k=0$ for $k<12$ and $\dim S_{12}=1$. See also [[ref-serre73]], VII.3, Théorème 4.

**Uses**: [[def-mk]], [[thm-lvl1-dims]].
