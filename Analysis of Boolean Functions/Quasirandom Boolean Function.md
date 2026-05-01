A function $f:\{ 0,1 \}^{n}\to \{ 0,1 \}$ is $(\epsilon,p,r)$-quasirandom
if for every $J\subseteq[n]$ of size $r$, and every $u\in \{ 0,1 \}^{J}$ 
$$
\left\lvert  \mathop{\mathbb{E}} (f^{(p)}(x) \mid x|_{J}=u) - \mathop{\mathbb{E}} f^{(p)}(x) \right\rvert \leq \epsilon
$$
### Intuition
Knowing what any $r$ coordinates of $x$ are gives almost no information to what $f(x)$ is going to be.

### Lemma
For every $\zeta>0$, $p\in\left[ \zeta,\frac{1}{2}-\zeta \right]$ and $\alpha>0$ 
there is some $\epsilon,r$ such that if $\mathop{\mathbb{E}}f^{(p)}=\alpha$ for some monotone $f:\{ 0,1 \}^{n}\to \{ 0,1 \}$
and $f$ is $(\epsilon,p,r)$-quasirandom then
$$
\mathop{\mathbb{E}}f^{(1/2)}>\frac{1}{2}
$$
(actually $>1-\delta$ for $\delta>0$)
#### Proof
Suppose that 
$$
\mathop{\mathbb{E}}f^{1/2} \leq \frac{1}{2}
$$
By the mean value theorem there is some $s \in\left( p,\frac{1}{2} \right)$ such that 
$$
\frac{d}{ds} \mathop{\mathbb{E}}f^{(s)} \leq \frac{ \frac{1}{2} -\alpha }{ \frac{1}{2}-p } \leq \frac{1}{\zeta}
$$
By [[Margulis-Russo Formula]] it follows
$$
I(f^{(s)}) \leq \frac{1}{\zeta}
$$
By the $s$-biased [[Friedgut Junta Theorem]] 
we can find a boolean $J$-[[Junta]] $h$ 
such that 
$$
\mathbb{P}(f^{(s)}\neq h^{(s)}) \leq \epsilon
$$
and $\lvert J \rvert\leq r(\zeta,\epsilon)$.
But
$$
\mathop{\mathbb{E}}f^{(s)} \leq \mathop{\mathbb{E}}f^{1/2} \leq \frac{1}{2}
$$
by monotonicity of $f$ so 
$$
\mathbb{P}(f^{(s)}=1) \leq \frac{1}{2} 
$$
