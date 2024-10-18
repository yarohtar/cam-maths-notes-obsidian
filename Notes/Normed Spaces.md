Let $X$ be a real or complex vector space. A norm of $X$ is a function $||\cdot||:X\to \mathbb{R}_{\geq 0}$ s.t.
1. $||x||=0 \iff x=0$
2. $||\lambda x||=|\lambda|\ ||x||$
3. $||x+y||\leq ||x||+||y||$
A normed space is a pair $(X,||\cdot||)$

NOTE: a normed space gives rise to a [[Metric spaces|metric space]] with $d(x,y)=||x-y||$. So we can talk about open sets, closed sets, convergent sequences etc.

[[L norms]]
### Unit ball
$B=\{x\in X : ||x||\leq 1\}$

Can check that $B$ is closed, bounded, convex, symmetric and a neighbourhood of 0.
Suppose $B'$ does satisfy this, then $B'$ defines a norm by taking
$||x||=\inf\left\{  \alpha\geq 0 \mid \frac{x}{\alpha}\in B'  \right\}$

[[Banach Space]]
[[Minkowski's Inequality]]
[[Hölder inequality]]

[[Metric spaces#Some properties]]

### Definition
We say topological space $X$ is separable if it has a countable dense subset.
#### Example
Each $l_{p}$ is separable for $1\leq p< \infty$ (take finite rational sequences). But $l_{\infty}$ is not separable.

### Definition
Norms $\lVert  \rVert_{1}$ and $\lVert  \rVert_{2}$ are equivalent if they induce the same topology.