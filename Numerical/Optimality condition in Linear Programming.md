Consider a [[Linear Program]] in the standard form:
" Minimize $c^Tx$ over $x\in \mathbb{R}^{n}$ subject to $Ax=b$ and $x\geq 0$ "
where $A\in \mathbb{R}^{m\times n}$, $c\in \mathbb{R}^{n}$ and $b\in \mathbb{R}^{m}$.
Suppose $x$ is a [[Basic Feasible Solution]] with [[Support]] $S\subseteq[n]$
Then $x$ is optimal
if and only if
$$
c - A^{T}\lambda \geq 0
$$
for some $\lambda \in \mathbb{R}^{m}$ satisfying $(A_{S}^{T})\lambda=c_{S}$
where $A_{B}$ is $m\times \lvert S \rvert$ submatrix of $A$
obtained by taking $i$-th columns of $A$ for all $i\in S$

Moreover, $\lambda$ is then feasible and optimal solution 
for the [[Dual Problem in Linear Programs]]:
" Maximize $\lambda^{T}b$ over $\lambda \in \mathbb{R}^{m}$ subject to $A^{T}\lambda\leq c$ "
### Proof
Start from the [[Dual Problem in Linear Programs]]:
" Maximize $\lambda^Tb$ over $\lambda \in \mathbb{R}^{m}$ subject to $A^{T}\lambda\leq c$ "
Note that a feasible $x$ is primal optimal 
and feasible $\lambda$ is dual optimal
if and only if 
[[Complimentary Slackness]] holds (due to [[Dual Problem in Linear Programs#Lemma]])
i.e. $x^{T}(c-A^{T}\lambda)=0$
i.e. $c_{S} - A_{S}^{T}\lambda=0$ (due to [[Support]] of $x$ being $S$)
#### $\implies$
Suppose $x$ is primal optimal.
By [[Strong duality in linear programs]], 
there is some feasible $\lambda$ that is dual optimal.
By the observation above, this means 
$$
c_{S}-A_{S}^{T}\lambda=0
$$
By feasibility of $\lambda$:
$$
c-A^{T}\lambda\geq 0
$$
#### $\impliedby$
Suppose some $\lambda$ satisfying $(A_{S}^{T})\lambda=c_{S}$ also satisfies:
$$
c-A^{T}\lambda\geq 0
$$
Then $\lambda$ is feasible, and $(c-A^{T}\lambda)x=0$ so [[Complimentary Slackness]] holds.
This happens if and only if $x$ is primal optimal and $\lambda$ is dual optimal.

## Corollary
Let $x$ be a [[Basic Feasible Solution]] with [[Support]] $B\subseteq[n]$
and suppose $\lvert B \rvert=m$ (i.e. $B$ is a [[Basis]] of $x$)
Then $x$ is optimal 
if and only if
$$
c-A^{T}((A_{B}^{T})^{-1}c_{B})\geq 0
$$
### Proof
Using the previous theorem, 
the unique $\lambda \in \mathbb{R}^{m}$ satisfying $(A_{B}^{T})\lambda=c_{B}$ is exactly:
$$
\lambda=(A_{B}^{T})^{-1}c_{B}
$$
where we used the fact that $A_{B}$ is square (due to $\lvert B \rvert=m$)
and invertible by the definition of [[Basic Solution]].
