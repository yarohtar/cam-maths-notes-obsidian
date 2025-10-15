Assume that the events $(A_{n})$ are [[Independence|independent]].
Suppose:
If $\sum_{n}\mathbb{P}(A_{n})=\infty$ then $\mathbb{P}(\lim\sup A_{n})=1$. ([[lim sup]])

The infinite monkey theorem follows from this.
#### Proof
Set $a_{n}=\mathbb{P}(A_{n})$. For all $n$ and $N\geq n$ we have:
$$
\mathbb{P}\left( \bigcap_{m=n}^N A_{m}^c \right) = \prod_{m=n}^{N} (1-a_{m})\leq \exp\left( -\sum_{m=n}^{N}a_{m} \right)\to 0
$$
where we used $1-a\leq \exp(-a)$
Hence $\mathbb{P}\left( \bigcap_{m\geq n}A_{m}^c \right)=0$ for all $n$
So $\mathbb{P}(\lim\sup A_{n})=1-\mathbb{P}\left( \bigcup _{n}\bigcap_{m\geq n}A_{m}^c \right)=1$
