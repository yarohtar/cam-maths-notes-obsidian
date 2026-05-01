A function $f:\{ 0,1 \}^{n}\to \{ 0,1 \}$ is $(\epsilon,p,r)$-quasirandom
if for every $J\subseteq[n]$ of size $r$, and every $u\in \{ 0,1 \}^{J}$ 
$$
\left\lvert  \mathop{\mathbb{E}} (f^{(p)}(x) \mid x|_{J}=u) - \mathop{\mathbb{E}} f^{(p)}(x) \right\rvert \leq \epsilon
$$
### Intuition
Knowing what any $r$ coordinates of $x$ are gives almost no information to what $f(x)$ is going to be.
