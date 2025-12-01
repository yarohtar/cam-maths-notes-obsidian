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


