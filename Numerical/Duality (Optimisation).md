We are solving the problem 
" Minimize $f(x)$ subject to $g(x)=b$, $x\in X$ "
Define [[Numerical/Lagrangian|Lagrangian]]:
$$L(x,\lambda)=f(x)-\lambda^T(g(x)-b)$$
Now we define the dual problem: 
" Maximize $h(\lambda)=\inf_{x\in X}L(x,\lambda)$ subject to $\lambda\in \Lambda$ "
where $\Lambda$ is the set of [[Feasible Lagrange Multipliers]]

### Weak duality
$$\sup_{\lambda\in\Lambda}h(\lambda)\leq \inf_{x\in X,\ g(x)=b}f(x)$$
#### Proof
Note:
$$
\inf_{x\in X}L(x,\lambda) \leq \inf_{x\in X, g(x)=b}L(x,\lambda)=\inf_{x\in X,g(x)=b}f(x)
$$
Thus
$$
\sup_{\lambda \in \Lambda}h(\lambda)\leq \inf_{x\in X,g(x)=b}f(x)
$$

### Strong duality
By [[Lagrange sufficiency theorem]]
If $x^*$ and $\lambda^*$ are feasible for primal and dual problem respectively, 
and $h(x^*)=f(x^*)$ 
then $x^*$ is optimal.

