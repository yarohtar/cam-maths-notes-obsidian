Let $\mathbb{P}$ be a [[Forcing Partial Order]].
Let $\lambda$ be an [[Ordinal]].
A [[Name]] $\tau$ is a nice name for subsets of $\lambda$
if there is a family $\mathcal{R}=\{ A_{\alpha}:\alpha<\lambda \}$ 
such that $A_{\alpha}$ is a [[Maximal Strong Antichain]] and 
$$
\tau=\tau_{\mathcal{R}}=\{ (\check{\alpha},p) : \alpha<\lambda \land p\in A_{\alpha} \}
$$
## Theorem
Let $G$ be a $\mathbb{P}$-[[Generic Filter]] over a [[Transitive Model]] $M\models ZFC$.
Then every subset of $\lambda$ in $M[G]$ has a nice name in $M$.
### Proof
Fix $\mu^{G}\subseteq \lambda$ for some [[Name]] $\mu \in M$.
Suppose that $\mu$ is not a nice name.
Fix $\alpha<\lambda$.
Then $\alpha^{G}\in \mu^{G}$ if and only if some $p\in G$ forces $\alpha \in \mu$.
Using [[Zorn's Lemma]] in $M$, 
build a [[Maximal Strong Antichain]] $A_{\alpha}\subseteq \mathbb{P}$ such that 
$$
(\forall p\in A_{\alpha})\ p\Vdash \check{\alpha} \in \mu
$$
Thus we find 
$$
\mathcal{R}=\{ A_{\alpha} : \alpha<\lambda \}\in M
$$
We now prove that
$$
\tau_{\mathcal{R}}^{G}= \mu^{G}
$$
which will finish the proof as $\tau_{\mathcal{R}}$ is a nice name.
#### $\subseteq$
If $\alpha \in \tau_{\mathcal{R}}^{G}$ then by definition there is $p\in G$ such that 
$$
(\check{\alpha},p)\in \tau_{\mathcal{R}}
$$
We conclude that $(\check{\alpha},p)\in A_{\alpha}$ so $p\Vdash \check{\alpha}\in \mu$.
Thus $\alpha \in \mu^{G}$.
#### $\supseteq$
If $\alpha \in \mathrm{val}(\mu,G)$, by [[Forcing Relation]] find $q\in G$ 
$$
q\Vdash \check{\alpha} \in \mu
$$
By the lemma in [[Dense Below]], if $G\cap A_{\alpha}=\varnothing$ 
then $A_{\alpha}\cup \{ q \}$ is a larger antichain with $(\forall s)\,s\Vdash \check{\alpha}\in \mu$.
Therefore, we could have WLOG taken $q\in G\cap A_{\alpha}$.
But then $(\check{\alpha},q)\in \tau_{\mathcal{R}}$ so 
$$
\alpha \in \mathrm{val}(\tau_{\mathcal{R}},G)
$$
