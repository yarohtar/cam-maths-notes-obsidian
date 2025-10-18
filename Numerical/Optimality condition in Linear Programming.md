Consider a [[Linear Program]] in the standard form:
" Minimize $c^Tx$ over $x\in \mathbb{R}^{n}$ subject to $Ax=b$ and $x\geq 0$ "
where $A\in \mathbb{R}^{m\times n}$, $c\in \mathbb{R}^{n}$ and $b\in \mathbb{R}^{m}$.
Suppose $x$ is a [[Basic Feasible Solution]] with support $B\subseteq[n]$
Suppose that 
$$
x^{T}(I-A_{B}A) \geq 0
$$

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