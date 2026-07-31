---
id: a13f38fd0018
type: proposition
---

# Proposition — prop:theta-der

## Statement

> [!proposition] prop:theta-der
> We have
> $$
> \begin{aligned}
> H_2' &= \frac{1}{6} (H_{2}^{2} + 2 H_{2} H_{4} + E_2 H_2) \\
> H_3' &= \frac{1}{6} (H_{2}^{2} - H_{4}^{2} + E_2 H_3) \\
> H_4' &= -\frac{1}{6} (2H_{2} H_{4} + H_{4}^{2} - E_2 H_4) 
> \end{aligned}
> $$
> or equivalently,
> $$
> \begin{aligned}
> \partial_{2} H_{2} &= \frac{1}{6} (H_{2}^{2} + 2 H_{2} H_{4})  \\
> \partial_{2} H_{3} &= \frac{1}{6} (H_{2}^{2} - H_{4}^{2})  \\
> \partial_{2} H_{4} &= -\frac{1}{6} (2H_{2} H_{4} + H_{4}^{2}) 
> \end{aligned}
> $$

## Proof

> [!note]- Proof (click to expand)
> Equivalences are obvious from the definition of the Serre derivative.
> Define $f_{2}, f_{3}, f_{4}$ be the differences of the left and right hand sides of [[eq-h2-serre-der]], [[eq-h3-serre-der]], [[eq-h4-serre-der]].
> $$
> \begin{aligned}
> f_{2} &:= \partial_{2} H_{2} - \frac{1}{6} H_{2}(H_{2} + 2H_{4}) \\
> f_{3} &:= \partial_{2} H_{3} - \frac{1}{6} (H_{2}^2 - H_{4}^2) \\
> f_{4} &:= \partial_{2} H_{4} + \frac{1}{6} H_{4}(2H_{2} + H_{4}).
> \end{aligned}
> $$
> Then these are a priori modular forms of weight $4$ and level $\Gamma(2)$, and our goal is to prove that they are actually zeros.
> By Jacobi's identity [[eq-jacobi-identity]], we have $f_{2} + f_{4} = f_{3}$.
> Also, the transformation rules of $H_2, H_3, H_4$ give
> $$
> \begin{aligned}
> f_{2}|_{S} &= -f_{4} \\
> f_{2}|_{T} &= -f_{2} \\
> f_{4}|_{S} &= -f_{2} \\
> f_{4}|_{T} &= f_{3} = f_{2} + f_{4}.
> \end{aligned}
> $$
> Now, define
> $$
> \begin{aligned}
> g &:= (2 H_2 + H_4) f_2 + (H_2 + 2 H_4) f_4 \\
> h &:= f_{2}^{2} + f_{2}f_{4} + f_{4}^{2}.
> \end{aligned}
> $$
> Then one can check that both $g$ and $h$ are invariant under the actions of $S$ and $T$, hence they are modular forms of level $1$.
> Also, by analyzing the limit of $g$ and $h$ as $z \to i \infty$, one can see that $g$ and $h$ are cusp forms, hence $g = h = 0$ by [[eq-dims6]] and [[eq-dims8]].
> This implies
> $$
> \begin{aligned}
> 3 E_4 f_2^{2} &= 3 (H_2^2 + H_2 H_4 + H_4^2) f_2^{2} = ((2 H_2 + H_4)^{2} - (2H_2 + H_4)(H_2 + 2H_4) + (H_2 + 2H_4)^{2}) f_2^{2}\\
> &= (2 H_2 + H_4)^{2} (f_2^2 + f_2 f_4 + f_4^2) = 0
> \end{aligned}
> $$
> and by considering $q$-series ($E_4$ has an invertible $q$-series), we get $f_2 = 0$.
