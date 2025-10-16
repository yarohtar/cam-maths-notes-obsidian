Every [[Decipherable code]] satisfies [[Kraft's inequality]].
#### Proof
Let $f:\Sigma_{1}\to \Sigma_{2}^{*}$ be a decipherable code 
with word lengths $s_{1}\dots s_{m}$ and $s=\max s_{i}$
Let $r\in \mathbb{N}$
$$
\left( \sum_{i=1}^{m} a^{-s_{i}} \right)^{r}=\sum_{l=1}^{rs} b_{l}a^{-l}
$$
where $b_{l}$ is the number of ways of choosing $r$ codewords with total length $l$.

$f$ decipherable $\implies b_{l}\leq a^l$ 
(because any word of length $l$ in $\Sigma_{2}$ has at most one preimage under $f^{*}$ 
and there is $a^{l}$ such words)
Then
$$
\left( \sum_{i=1}^{m}a^{-s_{i}}  \right)^r\leq \sum_{i=1}^{rs}a^la^{-l}=rs
$$
Taking $r\to \infty$ we find:
$$
\sum_{i=1}^{m} a^{-s_{i}}\leq 1
$$

### Corollary 
A [[Decipherable code]] with prescribed word lengths exists 
if and only if
there exists a [[Prefix-Free Code]] with the same word lengths. 
