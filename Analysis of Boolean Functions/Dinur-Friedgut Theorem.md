For $p\in\left( 0,\frac{1}{2} \right)$ and $\epsilon>0$ there is some $T\in \mathbb{N}$ 
such that for any [[Intersecting Family]] $\mathcal{A}$ of subsets of $[n]$ 
there exists $J\subseteq[n]$ of size at most $T$ 
and an [[Intersecting Family]] $\mathcal{B}$ of subsets of $J$ 
such that 
$$
\mu_{p} (\mathcal{A}\setminus \bar{\mathcal{B}}) \leq \epsilon
$$
where $\bar{\mathcal{B}}$ is the [[Upward Closure]] of $\mathcal{B}$ (in terms of $\subseteq$).
#### Proof
Let $f:\{ 0,1 \}^{n}\to \{ 0,1 \}$.
Apply the [[Regularity Lemma for Boolean Functions]] with parameters $\left( \frac{\epsilon}{10},p,r,\frac{\epsilon}{2} \right)$ 
where $r$ is to be chosen.
That gives us some $J$ of size at most $T(\epsilon,p,r)$ such that if $u$ is chosen $\mu_{p}$-randomly from $\{ 0,1 \}^{J}$
then
$$
\mathbb{P}\left( f_{u}^{(p)} \text{ is not $\left( \frac{\epsilon}{10},p,r \right)$-QR} \right)\leq \frac{\epsilon}{2}
$$
Define 
$$
g:\{ 0,1 \}^{J} \to \{ 0,1 \}
$$
by setting $g(u)=1$ if $f_{u}^{(p)}$ is $\left( \frac{\epsilon}{10},p,r \right)$-[[Quasirandom Boolean Function]] and $\mathop{\mathbb{E}}f_{u}^{(p)}\geq \frac{\epsilon}{2}$ and $g(u)=0$ otherwise
Then 
$$
\mathbb{P}(f^{(p)}(x)=1 \land g(x|_{J})=0) \leq \frac{\epsilon}{2} + \frac{\epsilon}{2} = \epsilon
$$
(because we have $\frac{\epsilon}{2}$ for $f_{u}^{(p)}$ to not be quasirandom and another $\frac{\epsilon}{2}$ if its sparse)
This corresponds to the statement that
$$
\lvert \mathcal{A} \setminus \bar{\mathcal{B}} \rvert \leq \epsilon
$$