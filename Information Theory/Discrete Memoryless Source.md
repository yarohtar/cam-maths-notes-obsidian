A [[Source]] $\{ X_{n} \}$ taking values in a discrete set $A$ 
where all $X_{i}$ are identically distributed and independent
is called a Discrete Memoryless Source.
## Theorem
A DMS $\{ X_{n} \}$ satisfies [[Asymptotic Equipartition Property]] 
with entropy equal to [[Mathematical Entropy]] $H(X_{1})$
### Proof
Let $P$ be the distribution of $X_{1}$
and $P^{n}$ distribution of $X_{1}^{n}=(X_{1},\dots,X_{n})$
Then:
$$
\begin{gather}
P^{n}(X_{1}^{n})=\prod_{i=1}^{n}P(X_{i}) \\
-\frac{1}{n}\log P^{n}(X_{1}^{n}) = -\frac{1}{n}\sum_{i=1}^{n} \log P(X_{i})
\end{gather}
$$
Set $Y_{i}=-\log P(X_{i})$ 
and use [[Weak Law of Large Numbers]] for $n\to \infty$
to find:
$$
\frac{ 1 }{ n } \sum_{i=1}^{n} Y_{i} \xrightarrow{p} \mathbb{E}(Y_{i}) = H(X_{1})
$$
Hence $\{ X_{n} \}$ satisfies [[Asymptotic Equipartition Property]] with entropy $H(X_{1})$
