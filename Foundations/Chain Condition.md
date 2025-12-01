---
aliases:
  - c.c.
  - c.c.c.
---
A [[Forcing Partial Order]] $\mathbb{P}$ has the $\kappa$-chain condition 
if any [[Antichain]] $A$ in $\mathbb{P}$ has size $\lvert A \rvert<\kappa$.

If $\kappa=\aleph_{1}$ we call this the countable chain condition.
## Theorem
Let $M$ be a [[Model]] of $ZFC$ and 
$$
M\models \kappa\text{ is cardinal} \land \mathbb{P} \text{ has the }\kappa \text{-c.c.}
$$
Suppose we have a [[Model Extension]] $M[G]$ and $f\in M[G]$ such that 
$$
M[G] \models f:A\to B
$$
for some $A,B\in M$.
Then there is a function $F:A\to \mathcal{P}(B)$ such that $F\in M$ with 
$$
\begin{gather}
(\forall a\in A)\, f(a) \in F(a) \\
M\models(\forall a\in A)\, \lvert F(a) \rvert <\kappa
\end{gather}
$$ 
### Proof
Let $\tau$ be the [[Name]] for $f$ and $p\in \mathbb{P}$ with 
$$
p\Vdash\tau:\check{A}\to \check{B}
$$
Now define 
$$
F(a) =\{ b\in B:(\exists q\leq p)\, q\Vdash\tau(\check{a})=\check{b} \}
$$
Clearly $f(a)\in F(a)$ by the [[Forcing Relation]].
Clearly $F\in M$.
For each $b\in F(a)$, consider 
$$
\{ q\leq p : q\Vdash\tau(\check{a})=\check{b} \} \neq \varnothing
$$
Using [[Axiom of Choice]] in $M$, pick $q_{b}\leq p$ with $q_{b}\Vdash\tau(\check{a})=\check{b}$
Finally, write 
$$
Q_{b}=\{ q_{b}: b\in F(a) \} \in M
$$
We can check that $Q_{a}$ is an [[Antichain]].
But because $M\models \mathbb{P}\text{ has }\kappa\text{-c.c.}$ we conclude 
$$
M\models \lvert Q_{a} \rvert <\kappa
$$
But the function $b\to q_{b}$ is an injection from $F(a)$ to $Q_{a}$ thus 
$$
M\models \lvert F(a) \rvert <\kappa
$$
## Corollary
If $\kappa$ is a [[Regular Cardinal]] in $M$ and 
$$
M\models \mathbb{P}\text{ has }\kappa\text{-c.c.}
$$
then the [[Model Extension]] $M[G]$ has:
$$
M[G] \models \kappa\text{ is a cardinal}
$$
### Proof
Suppose not, so find $\lambda<\kappa$ with $f:\lambda \to \kappa$ surjective.
By above theorem, find $F:\lambda \to \mathcal{P}(\kappa)$ with $F\in M$ and 
$$
M\models(\forall \alpha<\lambda)\, \lvert F(\alpha) \rvert <\kappa \land f(\alpha)\in F(\alpha)
$$
We conclude 
$$
\mathrm{ran}(f) \subseteq \bigcup_{\alpha<\lambda} F(\alpha)
$$
This contradicts that $\kappa$ is [[Regular Cardinal]]
