A set $x$ is transitive if every memeber of a member of $x$ is in $x$ i.e.
$$
(\forall y)((\exists z)(z\in x \land y\in z)\implies y\in x)
$$
Equivalently 
$$
\bigcup x\subseteq x
$$

### Lemma
$$
(\forall x)(\exists t)(t\text{ is transitive}\land(x\subseteq t))
$$
#### Proof
We define '$f$ is an attempt' to mean '$f$ is a function' and $(dom\ f\in \omega)$ and $(f(0)=x)$ and
$$
(\forall n\in \omega)\left( n^{+}\in dom\ f \implies f(n^{+})=\bigcup f(n) \right)
$$
An easy $\omega$-ind