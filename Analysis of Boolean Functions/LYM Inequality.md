Let $1\leq r<s\leq n$ and let $\mathcal{A}\subseteq[n]^{(r)}$.
Write
$$
\partial_{s}\mathcal{A} = \{ B\in[n]^{(s)} : (\exists A\in \mathcal{A})\ A\subseteq B \}
$$
Then
$$
\frac{ \lvert \partial_{s} \mathcal{A} \rvert  }{ \binom{ n }{ s } } \geq \frac{ \lvert \mathcal{A} \rvert  }{ \binom{ n }{ r } }
$$
#### Proof
Let $\alpha=\frac{ \lvert \mathcal{A} \rvert }{ \binom{ n }{ r } }$ and $\beta=\frac{ \lvert \partial_{s}\mathcal{A} \rvert }{ \binom{ n }{ s } }$.
Define a bipartite graph by joining $A\in[n]^{(r)}$ to $B\in[n]^{(s)}$ if $A\subseteq B$.
Pick a random edge. 
The probability that it joins $\mathcal{A}$ to $\partial_{s}\mathcal{A}$ is $\alpha$.
It is also at most $\beta$.
So $\alpha\leq \beta$.
lol
### Modified version
Let also $J\subseteq[n]$ and define
$$
\partial_{J}^{s} \mathcal{A} = \{ B\in[n]^{(s)} : (\exists A\in \mathcal{A})\ A\subseteq B\land (B\setminus A)\cap J=\varnothing \}
$$
Let 
$$
\alpha=\frac{ \lvert \mathcal{A} \rvert  }{ \binom{ n }{ r } }\quad %quad
\text{ and }\quad %quad
\beta=\frac{ \lvert \partial_{J}^{s}\mathcal{A} \rvert  }{ \binom{ n }{ s } }
$$
Assume that $r\leq \frac{n}{2}-\lvert J \rvert$.
Then
$$
\beta\geq \alpha\left( 1- \frac{ 2\lvert J \rvert  }{ n } \right)^{s-r}
$$
#### Proof
Pick a random pair $A\in[n]^{(r)}$, $B\in[n]^{(s)}$ with $A\subseteq B$.
Then $\mathbb{P}(A\in \mathcal{A})=\alpha$ and $B$ adds $s-r$ random elements from $[n]\setminus A$.
Each of them has probability 
$$
\mathbb{P}((A,B)\in \mathcal{A}\times \partial_{J}^{s}\mathcal{A}) \geq \alpha\left( 1-\frac{ 2\lvert J \rvert  }{ n } \right)^{s-r}
$$

