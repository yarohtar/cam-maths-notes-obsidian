Consider the primal problem:
" Minimize $c^Tx$ s.t. $Ax=b$ $x\geq 0$ "
Now the [[Numerical/Lagrangian|Lagrangian]] is:
$$
L(x,\lambda)=c^Tx-\lambda^T(Ax-b)=(c^T-\lambda^TA)x+\lambda^T b
$$
The set of [[Feasible Lagrange Multipliers]] is:
$$
\Lambda=\{c^T-\lambda^TA\geq 0\}=\{\lambda:\lambda^TA\leq c^T\}
$$
and finally, the [[Dual Problem]] function is:
$$
h(\lambda)=\inf_{x\geq 0}(c^T-\lambda^TA)x+\lambda^Tb=\lambda^Tb
$$
So the dual problem is:
" Maximize $\lambda^Tb$ over $\lambda$ subject to $\lambda^TA\leq c^T$ "

Note that this is a [[Linear Program]] in [[Forms of linear programs#General form|General Form]].

If we try to find the dual problem of the dual problem, 
we should end up with the primal problem. 
