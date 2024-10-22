Suppose we have a numerical method of the form
$$
u^{n+1}=A_hu^{n}
$$
and an exact solution $\hat{u}$.
The method is consistent if:
$\hat{u}^{n+1}=A_{h}\hat{u}^+\eta^n$ and $\lVert \eta^n \rVert=O(k^2)$. $\eta^n$ is called the local truncation error, while $k$ is the time step.
