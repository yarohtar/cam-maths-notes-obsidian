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
