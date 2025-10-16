Let $\{ X_{n} \}$ be a [[Source]] taking values in a discreet set $A$
It satisfies the AEP with constant $H\geq 0$ if:
for all $\epsilon>0$ and all large enough $n$:
$$
\mathbb{P}(X_{1}^{n}\in B_{n}^{*}(\epsilon)) > 1-\epsilon
$$
where $B_{n}^{*}(\epsilon)$ is the set of [[Typical Strings]].

### Lemma
Let $\{ X_{n} \}$ be a [[Source]] taking values in a discrete set $A$
Let $P^{n}:\mathbb{A}^{n}\to[0,1]$ be the joint PDF of $(X_{1},\dots,X_{n})$:
$$
P^{n}(x_{1}^{n})=\mathbb{P}(X_{1}^{n}=x_{1}^{n})
$$
for all $x_{1}^{n}\in A^{n}$
Then $\{ X_{n} \}$ satisfies AEP for $H\geq 0$
if and only if 
$$
-\frac{1}{n}\log P^n(X_{1},\dots,X_{n}) \xrightarrow{p} H
$$
as $n\to \infty$ where $\xrightarrow{p}$ means [[Convergence in Probability]]
This comes from [[Shannon's 1st coding theorem]]
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
If $n$ is large enough, then this happens with probability:
$$
\mathbb{P}\left( \left\lvert  \frac{1}{n} \log P^{n}(X_{1}^{n}) + H  \right\rvert \leq \epsilon \right) > 1-\epsilon
$$
Define:
$$
Q_{n}(\epsilon) = \mathbb{P}\left( \left\lvert  \frac{1}{n}\log P^{n} (X_{1}^{n}) + H  \right\rvert >\epsilon \right)
$$
We have proved that for any $\epsilon>0$:
$$
\lim_{n\to \infty} Q_{n}(\epsilon) < \epsilon
$$


### Proposition
A [[Bernoulli Source]] satisfies AEP with information rate $H(X)$ 
for $H(X)$ [[Mathematical Entropy]].
