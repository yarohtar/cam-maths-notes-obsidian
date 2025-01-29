The minimum expected word length of a decipherable code $f:\Sigma_{1}\to \Sigma_{2}^{*}$ satisfies
$$
\frac{H(X)}{\log a}\leq E(S)<\frac{H(X)}{\log a}+1
$$
#### Proof
The lower bound is given by combining [[Gibbs' inequality]] and [[Kraft's inequality]].
Take $q_{i}=\frac{a^{-s_{i}}}{C}$ where $C$ is just the normalizing factor.

$$
\begin{align}
H(X) & =-\sum_{i=1}^{m} p_{i}\log p_{i} \\
 & \leq-\sum_{i=1}^{m} p_{i}\log p_{i} \\
 & =\sum_{i=1}^{m}p_{i}s_{i}\log a +\sum p_{i}\log C \\
 & \leq \left( \sum_{i=1}^{m} p_{i}s_{i} \right)\log a +\log C
\end{align}
$$
Where $\log C\leq 0$ by [[Kraft's inequality]].
Hence:
$$
\frac{H(X)}{\log a}\leq \sum_{i=1}^{m} p_{i}s_{i}=E(S)
$$
We get equality iff $p_{i}=a^{-s_{i}}$ for some integers $s_{i}$.