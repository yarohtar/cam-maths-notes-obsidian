Suppose we reach a system:
$$
u' = Au
$$
where $u(0)=u_{0}$ and $A$ is a matrix.
(For example, by [[Semidiscretization]])
The solution is given by:
$$
u(t) = e^{tA} u_{0}
$$
If $A$ can be diagonalized as $A=VDV^{-1}$, 
then $e^{tA}=Ve^{tD}V^{-1}$ where $e^{tD}=\operatorname{diag}(e^{tD_{ii}})$
Computing such an eigenvalue decomposition can be expensive
We have a couple approximations

$e^{z} = 1+z+O(z^{2})$ gives [[Euler method]]
$$
u^{n+1} = (I+kA) u^{n}
$$