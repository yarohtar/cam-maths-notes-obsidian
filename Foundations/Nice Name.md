Let $\mathbb{P}$ be a [[Forcing Partial Order]].
Let $\lambda$ be an [[Ordinal]].
A [[Name]] $\tau$ is a nice name for subsets of $\lambda$
if there is a family $\mathcal{R}=\{ A_{\alpha}:\alpha<\lambda \}$ 
such that $A_{\alpha}$ is a [[Maximal Antichain]] and 
$$
\tau=\tau_{\mathcal{R}}=\{ (\check{\alpha},p) : (\exists \alpha<\lambda)\,A_{\alpha}\in \mathcal{R} \land p\in A_{\alpha} \}
$$
## Theorem
Let $G$ be a $\mathbb{P}$-[[Generic Filter]] over a [[Model]] $M\models ZFC$.
Then every subset of $\lambda$ in $M[G]$ has a nice name.
### Proof
Fix $x=\mathrm{val}(\mu,G)$ for some $\mu$.
Suppose that $\mu$ is not a nice name.
Fix $\alpha<\lambda$.
Using [[Zorn's Lemma]] in $M$, build a [[Maximal Antichain]] $A_{\alpha}\subseteq \mathbb{P}$ such that 
$$
(\forall p\in A_{\alpha})\, p\Vdash \check{\alpha} \in \mu
$$ 
Thus we find 
$$
\mathcal{R}=\{ A_{\alpha} : \alpha<\lambda \}\in M
$$
#### Claim
$$
\mathrm{val}(\tau_{\mathcal{R}},G) = \mathrm{val}(\mu,G)
$$
##### $\subseteq$
If $\alpha \in \mathrm{val}(\tau_{\mathcal{R}},G)$ then by definition there is $p\in G$ such that 
$$
(\check{\alpha},p)\in \tau_{\mathcal{R}}
$$
We conclude that $(\check{\alpha},p)\in A_{\alpha}$ so $p\Vdash \check{\alpha}\in \mu$.
Thus $\alpha \in \mathrm{val}(\mu,G)$.
##### $\supseteq$
If $\alpha \in \mathrm{val}(\mu,G)$, by [[Forcing Relation]] find $q\in G$ 
$$
q\Vdash \check{\alpha} \in \mu
$$
[[Generic Filter]]