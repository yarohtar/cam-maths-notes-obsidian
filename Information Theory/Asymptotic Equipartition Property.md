Let $\{ X_{n} \}$ be a [[Source]].
It satisfies the AEP with constant $H\geq 0$ if:
for all $\epsilon>0$ and all large enough $n$:
$$
\mathbb{P}(X_{1}^{n}\in B_{n}^{*}(\epsilon)) > 1-\epsilon
$$
where $B_{n}^{*}(\epsilon)$ is the set of [[Typical Strings]].

### Lemma
Let $\{ X_{n} \}$ be a source taking values in a discrete set $A$
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

### Definition 2
A [[Source]] $X_{1},X_{2},\dots$ satisfies AEP if for some $H\geq 0$
$$
-\frac{1}{n}\log P(X_{1},\dots,X_{n})\to^pH
$$
where $\to ^{p}$ means 'converges in probability'. 
So we can take very different values for large $n$, 
but only on a set of small probabilities

This second definition comes from [[Shannon's 1st coding theorem]]

### Proposition
A [[Bernoulli Source]] satisfies AEP with information rate $H(X)$ 
for $H(X)$ [[Mathematical Entropy]].
