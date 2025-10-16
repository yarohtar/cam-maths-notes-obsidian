Let $\{ X_{n} \}$ be a [[Source]] taking values in a discrete set $A$
Let $P^{n}:A^{n}\to[0,1]$ be the joint PDF of $(X_{1},\dots,X_{n})$:
$$
P^{n}(x_{1}^{n})=\mathbb{P}(X_{1}^{n}=x_{1}^{n})
$$
for all $x_{1}^{n}\in A^{n}$ 
(using notation $X_{1}^{n}=(X_{1},\dots,X_{n})$)
Then $\{ X_{n} \}$ satisfies AEP with entropy $H\geq 0$ if:
$$
-\frac{1}{n}\log P^n(X_{1}^{n}) \xrightarrow{p} H \quad %quad
\text{as }n\to \infty
$$
where $\xrightarrow{p}$ means [[Convergence in Probability]]
and $P^{n}(X_{1}^{n})$ is [[Random Probability of Random Variable]]
##### Note
There are alternative definitions, e.g. based on [[Typical Strings]].
However, this definition made the most sense to me, so I'm using it as main.
Sometimes, this is stated as a theorem instead, 
but I find that not very elegant.
[[Interpretation of Asymptotic Equipartition Property]]
## Theorem
Suppose $\{ X_{n} \}$ satisfies AEP with entropy $H\geq 0$.
Then the smallest sets of strings $B_{n}\subseteq A^{n}$
that hits $X_{n}$ almost surely has size $\approx2^{nH}$

Then there are around $2^{nH}$ [[Typical Strings]].
More precisely:
$$
(1-\epsilon)2^{n(H-\epsilon)} \leq \lvert B_{n}^{*}(\epsilon) \rvert \leq 2^{n(H+\epsilon)}
$$
### Proof
Let $\epsilon>0$.
From [[Typical Strings]], we know $\lvert B_{n}^{*}(\epsilon) \rvert\leq 2^{n(H+\epsilon)}$ 
(regardless of whether AEP is satisfied)
The other inequality follows from the following lemma.
### Lemma
Let $\{ X_{n} \}$ be a [[Source]] taking values in a discreet set $A$
Suppose $\{ X_{n} \}$ satisfies AEP with entropy $H\geq 0$
Let $\{ B_{n} \}$ be any sequence of subsets of $A^{n}$
Suppose
$$
\mathbb{P}(X_{1}^{n} \in B_{n})\to 1 \quad %quad
\text{as } n\to \infty 
$$
Then for any $\epsilon>0$ and any large enough $n$:
$$
\lvert B_{n} \rvert \geq(1-\epsilon) 2^{n(H-\epsilon)}
$$
#### Proof




### Proposition
A [[Bernoulli Source]] satisfies AEP with information rate $H(X)$ 
for $H(X)$ [[Mathematical Entropy]].
