Let $K$ be an [[Algebraically Closed Field]].
Suppose that the function $\Phi:K^{n}\to K^{n}$ is an injective [[Polynomial Map]].
Then $\Phi$ is surjective.
### Proof
First suppose 
$$
K=\bigcup_{k} \mathbb{F}_{p^{k}}
$$
for some prime $p$.
Fix some $m$ such that all coefficients of $\Phi$ come from $\mathbb{F}_{p^{m}}$.
Then for any $k\geq 1$, $\Phi$ induces an injective polynomial map $\mathbb{F}_{p^{km}}^{n}\to \mathbb{F}_{p^{km}}^{n}$
which has to be surjective since $\mathbb{F}_{p^{km}}$ is finite.
Hence 
$$
\Phi(K) = \Phi\left( \bigcup_{k} \mathbb{F}_{p^{km}}^{n} \right) =\bigcup_{k} \Phi(\mathbb{F}_{p^{km}}^{n}) = \bigcup_{k} \mathbb{F}_{p^{}}
$$