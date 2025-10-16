Let $\{ X_{n} \}_{n\in \mathbb{N}}$ be random variables taking values in alphabet $A$
and let $H\geq 0$
The sets of typical strings of length $n\in \mathbb{N}$ with constant $H$
are defined for each $\epsilon>0$ by:
$$
B_{n}^{*}(\epsilon)= \{ x_{1}^{n}\in A^{n} : 2^{-n(H+\epsilon)} \leq P^{n}(x_{1}^{n}) \leq 2^{-n(H-\epsilon)} \}
$$
where $P^{n}$ is the joint probability density function for $X_{1}^{n}=(X_{1},\dots,X_{n})$

Usually, $H$ is [[Mathematical Entropy]] and $X_{n}$ are IID.

### Lemma
For any $H\geq 0$, any $\epsilon>0$, and any $n\geq 1$:
$$
\lvert B_{n}^{*}(\epsilon) \rvert \leq 2^{n(H+\epsilon)}
$$
#### Proof
Each $x_{1}^{n}\in B_{n}^{*}(\epsilon)$ has $P^{n}(x_{1}^{n})\geq 2^{-n(H+\epsilon)}$
Thus:
$$
1\geq \sum_{x_{1}^n\in B_{n}^{*}(\epsilon)} P^{n}(x_{1}^{n}) \geq \lvert B_{n}^{*}(\epsilon) \rvert 2^{-n(H+\epsilon)}
$$
