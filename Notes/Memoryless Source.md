A Bernoulli or memoryless [[Source]] is a sequence of
independently, identically distributed random variables, 
i.e. for each $\mu \in \Sigma_{1}$, $P(X_{i}=\mu)$ is independent of $i$ 
and independent of all previous and future symbols emitted
$$
P(X_{1}=\mu_{1},\dots,X_{k}=\mu_{k})=\prod_{i=1}^{k} P(X_{i}=\mu _{i})
$$
### Lemma
The [[Source Information Rate]] of a Bernoulli source is at most the expected word length of an [[Optimal Code]].
![[Pasted image 20250517175119.png]]
### Corollary
A Bernoulli source has information rate less than $H(X)+1$.
#### Proof
