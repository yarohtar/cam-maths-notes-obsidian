[[Expected word length]] for an [[Optimal Code]] $f$ satisfies:
$$
\frac{H(X)}{\log a}\leq E(S)<\frac{H(X)}{\log a}+1
$$
where $a=\lvert \Sigma_{2} \rvert$, and $H(X)$ is the  [[Mathematical Entropy]].

#### Proof
The lower bound is given by combining [[Gibbs' inequality]] and [[Kraft's inequality]].
Take $q_{i}=\frac{a^{-s_{i}}}{C}$ where $C$ is just the normalizing factor.

$$
\begin{align}
H(X) & =-\sum_{i=1}^{m} p_{i}\log p_{i} \\
 & \leq-\sum_{i=1}^{m} p_{i}\log q_{i} \\
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

For the upper bound, let $s_{i}=\lceil -\log_{a}p_{i} \rceil$
We have 
$$
-\log_{a}p_{i}\leq s_{i}<-\log_{a}p_{i}+1
$$
$$
\implies a^{-s_{i}}\leq p_{i}\implies \sum_{i=1}^{m} a^{-s_{i}}\leq \sum_{i=1}^{m} p_{i}=1
$$
So by [[McMillan's Theorem]] there is a prefix-free code with word lengths $s_{1},\dots,s_{m}$
Also
$$
\begin{align}
E(S) & =\sum_{i=1}^{m} p_{i}s_{i} \\
 & <\sum_{i=1}^{m} p_{i}(-\log_{a}p_{i}+1) \\
 & = \frac{H(X)}{\log_{a}}+1
\end{align}
$$
