---
id: db0009dece77
type: lemma
from: blueprint
lean:
  - H₂_T_action
  - H₃_T_action
  - H₄_T_action
  - H₂_S_action
  - H₃_S_action
  - H₄_S_action
formalized: true
---

# Lemma — lemma:theta-transform-S-T

## Statement

> [!lemma] lemma:theta-transform-S-T
> These elements act on the [[def-th00-th01-th10|theta functions]] in the following way
> $$
> \begin{aligned}
> H_2 | S &= -H_4  \\
> H_3 | S &= -H_3  \\
> H_4 | S &= -H_2 
> \end{aligned}
> $$
> and
> $$
> \begin{aligned}
> H_2 | T &= -H_2  \\
> H_3 | T &= H_4  \\
> H_4 | T &= H_3 
> \end{aligned}
> $$

## Proof

> [!note]- Proof (click to expand)
> The last three identities easily follow from the definition.
> For example, [[eq-h2-transform-t]] follows from
> $$
> \begin{aligned}
> \Theta_{2}(z + 1) &= \sum_{n\in\mathbb{Z}}e^{\pi i (n+\frac12)^2 (z + 1)}
> = \sum_{n \in \mathbb{Z}} e^{\pi i (n + \frac{1}{2})^{2}} e^{\pi i (n + \frac{1}{2})^{2} z} \\
> &= \sum_{n \in \mathbb{Z}} e^{\pi i (n^2 + n + \frac{1}{4})} e^{\pi i (n + \frac{1}{2})^{2} z} = \sum_{n \in \mathbb{Z}} (-1)^{n^2 + n}e^{\pi i / 4} e^{\pi i (n + \frac{1}{2})^{2} z} \\
> &= e^{\pi i / 4} \Theta_{2}(z)
> \end{aligned}
> $$
> and taking 4th power.
> [[eq-h2-transform-s]] and [[eq-h4-transform-s]] are equivalent under $z \leftrightarrow -1/z$, so it is enough to show [[eq-h2-transform-s]] and [[eq-h3-transform-s]].
> These identities follow from the identities of the *two-variable* Jacobi theta function, which is defined as (be careful for the variables, where we use $\tau$ instead of $z$)
> $$
> \theta(z, \tau) = \sum_{n \in \mathbb{Z}} e^{2 \pi i n z + \pi i n^2 \tau} 
> $$
> and already formalized by David Loeffler.
> This function specialize to the theta functions as
> $$
> \begin{aligned}
> \Theta_{2}(\tau) &= e^{\pi i \tau / 4} \theta(-\tau / 2, \tau)  \\
> \Theta_{3}(\tau) &= \theta(0, \tau)  \\
> \Theta_{4}(\tau) &= \theta(1/2, \tau)  \\
> \end{aligned}
> $$
> 
> Poisson summation formula gives
> $$
> \theta(z, \tau) = \frac{1}{\sqrt{-i \tau}} e^{-\frac{\pi i z^2}{\tau}} \theta\left(\frac{z}{\tau}, -\frac{1}{\tau}\right) 
> $$
> and applying the specializations above yield the identities.
> For example, [[eq-h4-transform-s]] follows from
> $$
> \Theta_{4}(\tau) = \theta\left(\frac{1}{2}, \tau\right) = \frac{1}{\sqrt{-i\tau}} e^{- \frac{\pi i }{4 \tau}} \theta\left(\frac{1}{2 \tau}, -\frac{1}{\tau}\right) = \frac{1}{\sqrt{-i\tau}} \Theta_{2}\left(-\frac{1}{\tau}\right)
> $$
> and taking 4th power.
