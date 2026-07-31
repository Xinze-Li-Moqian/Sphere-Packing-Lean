---
id: 163185c6e61b
type: theorem
from: blueprint
lean:
  - LinearProgrammingBound'
formalized: true
---

# Theorem — Cohn–Elkies [[ref-elkiescohn]]

## Statement

> [!theorem] Cohn–Elkies [[ref-elkiescohn]]
> Let $X\subset\mathbb{R}^d$ be a discrete subset such that $\|x-y\|\geq 1$ for any distinct $x,y\in X$. Suppose that $X$ is $\Lambda$-[[periodicspherepacking|periodic]] with respect to some [[iszlattice|lattice]] $\Lambda\subset\mathbb{R}^d$. Let $f:\mathbb{R}^d\to\mathbb{R}$ be a [[def-schwartz-space|Schwartz function]] that is not identically zero and satisfies the following conditions:
> $$f(x)\leq 0\mbox{ for } \|x\|\geq 1$$ and
> $$\widehat{f}(x)\geq0\mbox{ for all } x\in\mathbb{R}^d.$$
> Then the [[spherepackingdensity|density]] of any $\Lambda$-periodic [[spherepackingballs|sphere packing]] is bounded above by $$\frac{f(0)}{\widehat{f}(0)}\cdot \mathrm{vol}(B_d(0,1/2)).$$

## Proof

> [!note]- Proof (click to expand)
> Here we reproduce the proof given in [[ref-elkiescohn]].
> 
> The inequality
> $$
> \sharp (X/\Lambda)\cdot f(0)\geq \sum_{x\in X}\sum_{y\in X/\Lambda}f(x-y)=\sum_{x\in X/\Lambda}\sum_{y\in X/\Lambda}\sum_{\ell\in  \Lambda}f(x-y+l)$$
> follows from the condition [[eq-cohn-elkies-condition-1]] of the theorem and the assumption on the distances between points in $X$.
> The equality
> $$\sum_{x\in X/\Lambda}\sum_{y\in X/\Lambda}\sum_{\ell\in  \Lambda}f(x-y+l)=\sum_{x\in X/\Lambda}\sum_{y\in X/\Lambda}\frac{1}{\mathrm{vol}(\mathbb{R}^d/\Lambda)}\,\sum_{m\in \Lambda^*} \widehat{f}(m)\,e^{2\pi i m(x-y)}.$$
> follows from the Poisson summation formula.
> The right hand side of the above equation can be written as
> $$\sum_{x\in X/\Lambda}\sum_{y\in X/\Lambda}\frac{1}{\mathrm{vol}(\mathbb{R}^d/\Lambda)}\,\sum_{m\in \Lambda^*} \widehat{f}(m)\,e^{2\pi i m(x-y)}=\frac{1}{\mathrm{vol}(\mathbb{R}^d/\Lambda)}\,\sum_{m\in \Lambda^*} \widehat{f}(m)\cdot\big|\sum_{x\in X/\Lambda}e^{2\pi i m x}\big|^2.$$
> Note that $\big|\sum_{x\in X/\Lambda}e^{2\pi i m x}\big|^2\geq0$ for all $m\in\Lambda^*$. Moreover,  the term corresponding to $m=0$ satisfies $\big|\sum_{x\in X/\Lambda}e^{2\pi i 0 x}\big|^2=\sharp (X/\Lambda)^2$.
> Now we use the condition [[eq-cohn-elkies-condition-2]] and estimate
> $$\frac{1}{\mathrm{vol}(\mathbb{R}^d/\Lambda)}\,\sum_{m\in \Lambda^*} \widehat{f}(m)\cdot\big|\sum_{x\in X/\Lambda}e^{2\pi i m(x-y)}\big|^2
> \geq \frac{\sharp (X/\Lambda)^2}{\mathrm{vol}(\mathbb{R}^d/\Lambda)}\cdot \widehat{f}(0).
> $$
> Comparing inequalities (eqn: sharp X 1) and (eqn: sharp X 2) we arrive at
> $$\frac{\sharp (X/\Lambda)}{\mathrm{vol}(\mathbb{R}^d/\Lambda)}\leq \frac{f(0)}{\widehat{f}(0)}.$$
> Now we see that the density of the [[periodicspherepacking|periodic packing]] $\mathcal{P}_X$ with balls of radius $1/2$ is bounded by
> $$\Delta(\mathcal{P}_X)=\frac{\sharp (X/\Lambda)}{\mathrm{vol}(\mathbb{R}^d/\Lambda)}\cdot{\mathrm{vol}(B_d(0,1/2))}\leq
> \frac{f(0)}{\widehat{f}(0)}\cdot \mathrm{vol}(B_d(0,1/2)).$$
> This finishes the proof of the theorem for periodic packings.
