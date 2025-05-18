Let $C$ be a [[Cyclic Code]] of length $n$ 
with [[Generator Polynomial]] $g\in \mathbb{F}_{2}[X] /(X^{n}-1)$
Let $K$ be a field extension of $\mathbb{F}_{2}$ containing all $n$-th roots of unity
(e.g. $K=\mathbb{F}_{2^{r}}$ for $2^{r}=1\pmod{n}$, or $K$ a [[Splitting Field]] of $X^{n}-1$)
The defining set of $C$ is then:
$$
A=\{ \alpha \in K:\alpha^{n}=1\land g(\alpha)=0 \}
$$
Note that the exact choice of $K$ won't matter,
as long as it does contain all $n$-th roots of unity.
### Lemma
Let $K$ be any field extension of $\mathbb{F}_{2}$
Let $A\subseteq \{ \alpha \in K : \alpha^{n}=1\}$
Then there is a unique code $C$ such that $A$ is it's defining set.
Moreover:
$$
C=\{ g\in \mathbb{F}_{2}[X] /(X^{n}-1) : (\forall \alpha \in A)\ g(\alpha)=0  \}
$$
#### Proof



# This wasn't done in lectures like this
See [[Cyclic Code with Defining Set]]