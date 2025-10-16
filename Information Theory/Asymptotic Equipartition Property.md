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
and $P^{n}(X_{1}^{n})$ is "random probability of random string".
##### Note
There are alternative definitions, e.g. based on [[Typical Strings]].
However, this definition made the more sense to me, so I'm using it as main.
##### Interpretation
We are saying that $\{ X_{n} \}$ satisfies AEP if, 
for large enough $n$,
given a random string $X_{1}^{n}$,
the probability that 
## Lemma
Let $\{ X_{n} \}$ be a [[Source]] taking values in a discreet set $A$
It satisfies the AEP with constant $H\geq 0$ if:
for all $\epsilon>0$
$$
\lim_{n\to \infty}\mathbb{P}(X_{1}^{n}\in B_{n}^{*}(\epsilon)) = 1
$$
where $B_{n}^{*}(\epsilon)$ is the set of [[Typical Strings]] with entropy $H$
##### Note
There are some alternative definitions.
In this one, we make no claim that $H$ is the [[Mathematical Entropy]],
but it usually will be.
## Proposition
If $\{ X_{n} \}$ satisfies AEP with constant $H\geq 0$
Then for every $\epsilon$ 
### Lemma
#### Proof
Let $\epsilon>0$
Note that $X_{1}^{n}\in B_{n}^{*}(\epsilon)$ if and only if:
$$
2^{-n(H+\epsilon)} \leq P^{n}(X_{1}^{n}) \leq 2^{-n(H-\epsilon)}
$$
which happens if and only if:
$$
H-\epsilon\leq -\frac{1}{n} \log P^{n}(X_{1}^{n}) \leq H + \epsilon 
$$
Now $\{ X_{n} \}$ satisfies AEP
if and only if (by definition)
$$
\lim_{n\to \infty} \mathbb{P}\left( \left\lvert  \frac{1}{n} \log P^{n}(X_{1}^{n}) +H  \right\rvert > \epsilon \right) \to 0
$$
and [[Convergence in Probability]] follows.
### Lemma
Let $\{ X_{n} \}$ be a [[Source]] taking values in a discreet set $A$
Suppose $\{ X_{n} \}$ satisfies AEP with constant $H\geq 0$
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
