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
### Interpretation
Each string $x_{1}^{n}$ has probability $P^{n}(x_{1}^{n})$ of occurring
Choose one of the **probabilities** at random (following the distribution of $X_{1}^{n}$)
AEP says that this randomly chosen number is close to $2^{-nH}$ 
(with high probability).

In other words, most strings $x_{1}^{n}$ 
will have probability close to $2^{-nH}$.
These are called [[Typical Strings]].

There will usually be a lot of strings that are not typical.
We make no claims on whether they are more or less probable than $2^{-nH}$
However, seeing anything from the non typical set is improbable.
For example, consider $A=\{ 0,1 \}$ 
and $X_{n}$ are iid with $p_{0}=\frac{3}{4}$ and $p_{1}=\frac{1}{4}$.
We can find $H=2-\frac{3}{4}\log 3\approx 0.81$.
The string $0000\dots 0$ is the most probable, but not very "typical"
Indeed, it's probability is $p_{n}=2^{-2n}\cdot 3^{n}$ which gives:
$$
-\frac{1}{n}\log p_{n} = 2 - \log 3 \approx 0.42
$$
and that is not close to $H$.

where $B_{n}^{*}(\epsilon)$ is the set of [[Typical Strings]] with entropy $H$
## Proposition
If $\{ X_{n} \}$ satisfies AEP with constant $H\geq 0$
Then for every $\epsilon$ 
### Lemma
#### Proof
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
