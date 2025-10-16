Let $\{ X_{n} \}$ be a [[Random Variable]]s taking values in a discrete set $A$
Let $P^{n}:A^{n}\to[0,1]$ be the joint distribution of $(X_{1},\dots,X_{n})$:
$$
P^{n}(x_{1}^{n})=\mathbb{P}(X_{1}^{n}=x_{1}^{n})
$$
for all $x_{1}^{n}\in A^{n}$.
(using notation $X_{1}^{n}=(X_{1},\dots,X_{n})$)
Then $\{ X_{n} \}$ satisfies AEP with entropy $H\geq 0$ if:
$$
-\frac{1}{n}\log P^n(X_{1}^{n}) \xrightarrow{p} H \quad %quad
\text{as }n\to \infty
$$
where $\xrightarrow{p}$ means [[Convergence in Probability]]
and $P^{n}(X_{1}^{n})$ is [[Random Probability of Random Variable]]
##### Note
There are alternative definitions 
(e.g. based on [[Typical Strings#Lemma (AEP)]])
However, this definition made the most sense to me, so I'm using it as main.
Note also that I'm making no assumptions about $X_{n}$.
We can, however, prove that [[Discrete Memoryless Source]] satisfies AEP.
[[Interpretation of Asymptotic Equipartition Property]]
## Theorem
Suppose $\{ X_{n} \}$ satisfies AEP with entropy $H\geq 0$.
Then the smallest sets of strings $B_{n}\subseteq A^{n}$ such that:
$$
\mathbb{P}(X_{1}^{n}\in B_{n}) \xrightarrow{p} 1 \quad %quad
\text{as}\quad %quad
n\to \infty
$$
(where $\xrightarrow{p}$ is [[Convergence in Probability]])
have sizes $\lvert B_{n} \rvert\approx2^{nH}$.

More precisely, the following lemmata:
### Lemma 1
For every $\epsilon>0$
there is a sequence of sets $\{ B_{n}\subseteq A^{n} \}$ with $\lvert B_{n} \rvert\leq 2^{n(H+\epsilon)}$
such that:
$$
\mathbb{P}(X_{1}^{n}\in B_{n}) \xrightarrow{p} 1 \quad %quad
\text{as}\quad %quad
n\to \infty
$$
#### Proof
Let $\epsilon>0$.
Take $B_{n}=B_{n}^{*}(\epsilon)$, the sets of [[Typical Strings]] with entropy $H$.
We know that
$$
\lvert B_{n}^{*}(\epsilon) \rvert \leq 2^{n(H+\epsilon)}
$$
Also $\{ X_{n} \}$ satisfies AEP 
thus by [[Typical Strings#Lemma (AEP)]]:
$$
\mathbb{P}(X_{1}^{n}\in B_{n}^{*}(\epsilon)) \to ^{p} 1
$$
### Lemma 2
Let $\epsilon>0$.
Suppose for some $\{ B_{n}\subseteq A^{n} \}$ we have:
$$
\mathbb{P}(X_{1}^{n}\in B_{n}) \to ^{p} 1 \quad %quad
\text{as} \quad %quad
n\to \infty
$$
Then for all large enough $n$:
$$
(1-\epsilon)2^{n(H-\epsilon)} \leq \lvert B_{n} \rvert
$$
#### Proof
Using [[Inclusion-Exclusion Principle]]


### Proposition
A [[Memoryless Source]] satisfies AEP with information rate $H(X)$ 
for $H(X)$ [[Mathematical Entropy]].
