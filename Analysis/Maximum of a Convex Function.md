Let $S$ be a [[Compact]] [[Convex Set]].
Let $f:S\to \mathbb{R}$ be a nonconstant [[Convex Function]] that achieves its maximum.
Then $f$ achieves its maximum at an [[Extreme Point]] of $S$.
#### Proof
Suppose $f$ achieves its maximum at $x$.
Suppose $x$ is not an extreme point of $S$. 
Then $x=\lambda y+(1-\lambda)z$ for distinct $y\neq x$ and $z\neq x$ by definition of [[Convex Set]]
Then $f(x)\leq \lambda f(y)+(1-\lambda)f(z)$ by definition of a [[Convex Function]]
Because $f(x)\geq f(y),f(z)$ we have to have:
$$
f(x)=f(y)=f(z)
$$
In follows that, for any $\lambda \in \mathbb{R}$, 
if $t=z+\lambda(y-z)\in S$ then $f(t)=f(x)$

Now find the $\lambda'=\sup \{  \}$