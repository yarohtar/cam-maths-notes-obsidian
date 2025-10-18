Consider a [[Linear Program]] in the standard form:
" Minimize $c^Tx$ over $x\in \mathbb{R}^{n}$ subject to $Ax=b$ and $x\geq 0$ "
where $A\in \mathbb{R}^{m\times n}$, $c\in \mathbb{R}^{n}$ and $b\in \mathbb{R}^{m}$.
Suppose $x$ is a [[Basic Feasible Solution]] with [[Support]] $B\subseteq[n]$
Then $x$ is optimal
if and only if
$$
c - A^{T}\lambda \geq 0
$$
for some $\lambda \in \mathbb{R}^{m}$ satisfying $(A_{B}^{T})\lambda=c_{B}$
where $A_{B}$ is $m\times \lvert B \rvert$ submatrix of $A$
obtained by taking $i$-th columns of $A$ for all $i\in B$

Moreover, $\lambda$ is then feasible and optimal solution for the [[Dual Problem]].
### Proof
Start from the [[Dual problem in Linear Programs]]:
" Maximize $\lambda^Tb$ over $\lambda \in \mathbb{R}^{m}$ subject to $A^{T}\lambda\leq c$ "
Note that a feasible $x$ is primal optimal 
and feasible $\lambda$ is dual optimal
if and only if 
[[Complimentary slackness]] holds.
(due to [[Dual problem in Linear Programs#Lemma]])

Additionally, $x$ is optimal
if and only if
$x$ is a [[Basic Feasible Solution]]

Now suppose we can find $\lambda$ s.t.
- $(c^T-\lambda^TA)_{B(i)}=0$ [[Complimentary slackness]]
- $\lambda^TA\leq c^T$ feasibility of $\lambda$
Hence write:
$$\lambda^TB=c_B^T$$
$$B^T\lambda=c_B$$
$$\lambda=(B^T)^{-1}c_B$$
So as long as:
$$(c^T-c_B^TB^{-1}A)\geq 0$$
we can find such $\lambda$ and hence use [[Optimality condition in Linear Programming#Theorem|the theorem]] to finish.