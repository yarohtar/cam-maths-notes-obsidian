The $p$-biased cube is the set $\{ -1,1 \}^{n}$ with measure $\mu_{p}$
where for each $x\in \{ -1,1 \}^{n}$ we have $\mathbb{P}(x_{i}=-1)=p$, $\mathbb{P}(x_{i}=1)=q=1-p$ 
and 
$$
\mu=q-p = 1-2p
$$
$$
\sigma=2\sqrt{ pq }
$$
To normalize $x$ we introduce $\phi(x)$ where 
$$
\phi_{i}(x)=\frac{ x_{i}-\mu }{ \sigma }
$$
We will also write $\phi(t)=\frac{ t-\mu }{ \sigma }$ and 
$$
\phi_{A}(x) = \prod_{i\in A}\phi_{i}(x)
$$
(which are the [[Character]]s for this group)
For any $f,g:\{ -1,1 \}^{n}\to \mathbb{R}$ write
$$
\braket{ f | g } = \mathop{\Large\mathbb{E}}\limits_{x\sim \mu_{p}} f(x)g(x)
$$
Also define for $r \in[1,\infty]$:
$$
\lVert f \rVert _{r} = \left( \mathop{\Large\mathbb{E}}\limits_{x\sim \mu_{p}} \lvert f(x) \rvert ^{r} \right)^{1/r}
$$


