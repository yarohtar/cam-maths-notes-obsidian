Let $M$ be a [[Model]] of $ZFC$.
Let $(\mathbb{P},\leq,\mathbb{1})$ be a [[Forcing Partial Order]].
Let $F\subseteq \mathbb{P}$.
Then the model extension of $M$ by $F$ is 
$$
M[F] = \{ \mathrm{val}(\tau,F) : \tau \in \mathrm{Name}^{\mathbb{P}}\cap M \}
$$
where $\mathrm{Name}^{\mathbb{P}}$ are the $\mathbb{P}$-[[Names]], and $\mathrm{val}$ is the [[Value of a Name]].
### Lemma
If $M$ is countable [[Transitive Model|Transitive]], then so is $M[F]$.
#### Proof
Firstly $\mathrm{Name}^{\mathbb{P}}\cap M$ is countable, so $M[F]$ is countable.
By definition, it is also a [[Foundations/Set Theory/Transitive|Transitive]] set.
## Theorem
Let $M$ be a countable [[Transitive Model]] of $ZFC$
Let $(\mathbb{P},\leq,\mathbb{1})$ be a [[Forcing Partial Order]].
Let $F\subseteq \mathbb{P}$ be a [[Filter]] with $\mathbb{1}\in F$.
Then $M[F]$ is a countable [[Transitive Model]] of $ZFC$ 
and furthermore, $M\subseteq M[F]$ and $F\in M[F]$,
under certain conditions on $F$.
### Proof
Firstly, $M[F]$ is countable [[Transitive Model]] of $ZFC$ by above.
Secondly, we know that $M\subseteq M[F]$ and $F\in M[F]$ from [[Canonical Name]]s.

Any [[Transitive Model]] satisfies [[Axiom of Extensionality]] and [[Axiom of Foundation]].
Furthermore, as $\omega \in M\subseteq M[F]$, then $M[F]$ satisfies [[Axiom of Infinity]].

#### Pair
[[Pair-set axiom]]
Given $\sigma,\tau \in \mathrm{Name}^{\mathbb{P}}$, we need a name for 
$$
\{ \mathrm{val}(\sigma,F), \mathrm{val}(\tau,F) \} = \pi
$$
Set 
$$
\mathrm{up}(\sigma,\tau) = \{ (\sigma,\mathbb{1}), (\tau,\mathbb{1}) \}
$$
as the obvious name for the pair.
Then clearly: 
$$
\mathrm{val}(\mathrm{up}(\sigma,\tau), F) = \pi
$$
if $\mathbb{1}\in F$.
#### Union
[[Union axiom]]
Given $\sigma \in \mathrm{Name}^{\mathbb{P}}$ need a name for 
$$
\bigcup \mathrm{val}(\sigma,F)
$$
Define 
$$
u_{\sigma} = \Big\{ (\sigma',r) : (\exists \tau,p,q)\, (\tau,p)\in \sigma \land(\sigma',q)\in \tau \land r\leq p,q \Big\}
$$
We can check that if $F$ is a [[Filter]] then 
$$
\mathrm{val}(u_{\sigma},F) = \bigcup \mathrm{val} (\sigma,F)
$$
