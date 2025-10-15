Let $\{ X_{n} \}$ be a [[Source]].
It satisfies the Asymptotic Equipartition Property with constant $H\geq 0$ 
if for all $\epsilon>0$ 
there is some $n_{0}\in \mathbb{N}$ 
such that for all $n\geq n_{0}$ 
$$
\mathbb{P}(X_{1}^{n}\in B_{n}^{*}(\epsilon)) > 1-\epsilon
$$
where $B_{n}^{*}(\epsilon)$ is the set of [[Typical Strings]].

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
