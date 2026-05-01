Let $f:\mathbb{R}^{n}\to \mathbb{R}$ be a multilinear function.
Then
$$
\frac{d}{d\mu} \mathop{\mathbb{E}}f^{(p)} = \frac{1}{\sigma} \sum_{i=1}^{n} \hat{f}^{(p)}(i)
$$
where $f^{(p)}$ is always taken to be on the $p$-[[Biased Cube]].
#### Proof
We have 
$$
\mathop{\mathbb{E}}f^{(p)} = f(\mu, \dots, \mu)
$$
from the $p$-[[Biased Cube]]
Thus write 
$$
\begin{align}
\frac{d}{d\mu}\mathop{\mathbb{E}}f^{(p)}  & = \sum_{i=1}^{n} \frac{\partial}{\partial x_{i}} f(\mu, \dots, \mu) \\
 & = \sum_{i=1}^{n} \frac{1}{2}(f(\bar{\mu}_{i\to 1})-f(\bar{\mu}_{i\to-1})) \\
 & =
\end{align}
$$