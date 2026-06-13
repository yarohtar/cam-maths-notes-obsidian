Let $T$ be a [[Consistent]] [[Theory]].
Define the equivalence relation on formulas 
$\varphi \sim \psi$ if and only if $T\vdash (\varphi \iff \psi)$,
and for each $n\in \mathbb{N}$ fix variables $x_{1},x_{2},\dots,x_{n}$ let 
$$
F_{n}=\{ [\varphi]: \text{$\varphi$ has free variables $x_{1},\dots,x_{n}$}\}
$$
Clearly $F_{n}$ is a [[Boolean Algebra]].
An $n$-type over $T$ is a [[Boolean Algebra Ultrafilter]] on $F_{n}$,
i.e. some $p\subseteq F_{n}$ such that $p$ is [[Consistent]] 
and any $\varphi \in F_{n}$ has $[\varphi ] \in p$ or $[\neg \varphi ]\in p$.
These are the elements of the [[Formula Type Space]].
### Proposition
Let $\mathcal{M}$ be a [[Model]], $A\subseteq M$, and fix the language $\mathcal{L}_{A}$.
Let also $\bar{x}\in M^{n}$ and define 
$$
\mathrm{tp}(\bar{x} / A) = \{ [\varphi]: \mathcal{M}\models \varphi(\bar{x}) \}
$$
Then 
$$
\mathrm{tp}(\bar{x} / A) \in S_{n}^{\mathcal{M}}(A)
$$
Moreover, for any $p\in S_{n}^{\mathcal{M}}(A)$, 
there is an [[Elementary Extension]] $\mathcal{N}$ of $\mathcal{M}$
and some $\bar{x}\in N^{n}$ such that $p=\mathrm{tp}^{\mathcal{N}}(\bar{x} / A)$.
#### Proof
First bit is trivial.
Let $p\in S_{n}^{\mathcal{M}}(A)$. 
Then $p\in S_{n}(\mathrm{Th}_{A}(\mathcal{M}))$. 


