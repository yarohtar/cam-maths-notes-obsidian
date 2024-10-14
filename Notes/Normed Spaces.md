Let $X$ be a real or complex vector space. A norm of $X$ is a function $||\cdot||:X\to \mathbb{R}_{\geq 0}$ s.t.
1. $||x||=0 \iff x=0$
2. $||\lambda x||=|\lambda|\ ||x||$
3. $||x+y||\leq ||x||+||y||$
A normed space is a pair $(X,||\cdot||)$

NOTE: a normed space gives rise to a [[Metric spaces|metric space]] with $d(x,y)=||x-y||$. So we can talk about open sets, closed sets, convergent sequences etc.

Norms $L_p^n$ for any $1\leq p<\infty$ defined by $||X||_{p}=\left( \sum_{i=1}^{n}|X_{i}|^p \right)^{1/p}$ (by [[Minkowski's Inequality]])


### Unit ball
$B=\{x\in X : ||x||\leq 1\}$

Can check that $B$ is closed, bounded, convex, symmetric and a neighbourhood of 0, then $B$ does define a norm by $||x||=\inf\{t>0 : x\in tB\}$.

### Sequences
Let $S$ be the set of all scalar sequences (made into a vector space by coordinatewise addition)

$L_{p}$ stuff is defined on subsets of $S$ where they converge ... 

[[Banach Space]]
[[Hölder inequality]]
[[Minkowski's Inequality]]