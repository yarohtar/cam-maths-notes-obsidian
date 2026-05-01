Let $f:\{ 0,1 \}^{n}\to \mathbb{R}$ be a function on $p$-[[Biased Cube]] with $J\subseteq[n]$ and $u\in \{ 0,1 \}^{J}$.
Define $f_{u}:\{ 0,1 \}^{[n]\setminus J}\to \mathbb{R}$ by $f_{u}(y)=f(x)$ where $x|_{J}=u$ and $x|_{[n]\setminus J}=y$.
The averaging projection $E_{J}$ is defined by
$$
E_{J}f^{(p)}(x) = \mathop{\mathbb{E}}f_{u}^{(p)}
$$
where $u=x|_{J}$.
Note $E_{J}f(x)$ depends only on coordinates in $J$.
### Lemma
Each $E_{J}$ is an orthogonal projection and $$
