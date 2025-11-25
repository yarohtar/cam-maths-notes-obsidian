Let $(\mathbb{P},\leq,\mathbb{1})$ be a [[Forcing Partial Order]].
We define the $\mathbb{P}$-names by recursion: 
$$
\begin{gather}
\mathrm{Name}^{\mathbb{P}}_{0} = \varnothing  \\
\mathrm{Name}^{\mathbb{P}}_{\alpha+1} = \{ \tau : \tau \subseteq \mathrm{Name}^{\mathbb{P}}_{\alpha} \times \mathbb{P} \} \cup \mathrm{Name}^{\mathbb{P}}_{\alpha} \\
\mathrm{Name}^{\mathbb{P}}_{\lambda} = \bigcup_{\alpha<\lambda} \mathrm{Name}^{\mathbb{P}}_{\alpha} \\
\mathrm{Name}^{\mathbb{P}}=\bigcup_{\alpha \in \mathrm{Or d}} \mathrm{Name}^{\mathbb{P}}_{\alpha}
\end{gather}
$$
### Remark
When $\mathbb{P}=\{ \mathbb{1} \}$ then this is [[Von Neumann Hierarchy]].
### Interpretation
If $(\tau',p)\in \tau$ then $p$ guarantees that the set named by $\tau'$ is in the set named by $\tau$.

### Lemma
$\mathrm{Name}^{\mathbb{P}}$ is [[Absolute]].

