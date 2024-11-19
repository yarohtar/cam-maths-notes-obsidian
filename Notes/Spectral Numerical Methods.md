Consider a PDE of the form:
$$
\mathcal{L}u=f
$$
Consider the finite dimensional space of functions $V$ spanned by $\psi_{1},\psi_{2},\dots,\psi_{N}$.
We seek a solution of the form 
$$
u_{N}=\sum_{n=1}^Nc_{n}\psi_{n}
$$
In general, this does not exist, because there is no reason for $u$ to be in this span. So we only seek an approximation which satisfies:
$$
\sum_{n=1}^Nc_{n}\braket{ \mathcal{L}\psi_{n} | \psi_{m} } =\braket{ f | \psi_{m} }
$$
[[Four]]