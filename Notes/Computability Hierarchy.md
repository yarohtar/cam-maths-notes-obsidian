# $\Sigma_{1}$ sets
A set $X\subseteq \mathbb{B}^{k}$ is called $\Sigma_{1}$ if there is a [[Computable]] $Y\subseteq \mathbb{B}^{k+1}$ such that for all $\vec{w}\in \mathbb{B}^{k}$ we have
$$
\vec{w}\in X\iff \exists v((\vec{w},v)\in Y)
$$
### Proposition
The class of $\Sigma_{1}$ sets is not closed under complementation.
#### Proof
[[The Halting Problem]]
### Theorem
Let $X\subseteq \mathbb{B}^{k}$. The following are equivalent:
1. $X$ is [[Computably Enumerable]]
2. $X$ is $\Sigma_{1}$
# $\Pi_{1}$ sets
A set is called $\Pi_{1}$ if it is a complement of a $\Sigma_{1}$ set.
### Proposition
A set $X$ is $\Pi_{1}$ if and only if there is a [[Computable]] $Y\subseteq \mathbb{B}^{k+1}$ such that for all $\vec{w}\in \mathbb{B}^{k}$ we have
$$
\vec{w}\in X\iff \forall v(\vec{w},v) \in Y
$$
# $\Delta_{1}$ sets
A set is called $\Delta_{1}$ if it is both $\Sigma_{1}$ and $\Pi_{1}$.
### Proposition
A set is [[Computable]] if and only if it is a $\Delta_{1}$ set.

