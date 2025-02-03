A [[Source]] $X_{1},X_{2},\dots$ satisfies the Asymptotic Equipartition Property (AEP) with constant $H\geq 0$ if:
$$
\forall \epsilon>0 \exists n_{0}\in \mathbb{N} \forall n\geq n_{0}\exists T_{n}\subseteq \Sigma^{n}
$$
1. $$
P((X_{1},\dots,X_{n})\in T_{n})>1-\epsilon
$$
2. $$
2^{-n(H+\epsilon)}\leq P(x_{1},\dots,x_{n})\leq 2^{-n(H-\epsilon)}
$$
for all $(x_{1},\dots x_{n})\in T_{n}$

$T_{n}$ is called a typical set.


### Definition 2
A [[Source]] $X_{1},X_{2},\dots$ satisfies AEP if for some $H\geq 0$
$$
-\frac{1}{n}\log P(X_{1},\dots,X_{n})\to^pH
$$
where $\to ^{p}$ means 'converges in probability'. So we can take very different values for large $n$, but only on a set of small probabilities

This second definition comes from [[Shannon's 1st coding theorem]]

### Proposition
A [[Memoryless Source]] sastisfies AEP with information rate $H(X)$ fo