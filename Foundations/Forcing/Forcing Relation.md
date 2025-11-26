Let $M$ be a [[Transitive Model]] 
Let $\mathcal{L}_{\mathbb{P},M}$ be a [[Forcing Language]] with the [[Forcing Sentence]]s $\mathrm{Se nt}_{\mathbb{P},M}$.
A relation $\Vdash$ on $\mathbb{P}\times \mathrm{Se nt}_{\mathbb{P},M}$ is a forcing relation if 
for any $G$ that is a $\mathbb{P}$-[[Generic Filter]] over $M$,
the [[Model Extension]] $M[G]$,
any formula $\varphi \in \mathcal{L}_{\mathbb{P},M}$ with $k$ [[Free Variable]]s
and any [[Name]]s $\tau_{1},\dots,\tau_{k}\in \mathrm{Name}^{\mathbb{P}}\cap M$,
the following are equivalent: 
$$
\begin{gather}
M[G] \models \varphi(\mathrm{val}(\tau_{1},G),\dots,\mathrm{val}(\tau_{k},G)) \\
\iff \\
(\exists p\in G)\, M\models (p \Vdash \varphi(\tau_{1},\dots,\tau_{k}))
\end{gather}
$$
Additionally, we require that $\Vdash$ is downwards closed i.e. 
$$
p\Vdash \varphi \land q\leq p \implies q \Vdash \varphi
$$
