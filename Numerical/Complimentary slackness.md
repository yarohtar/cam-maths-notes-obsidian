Suppose we are minimizing (over $x$ and $s$) the [[Numerical/Lagrangian|Lagrangian]]
$$
L(x,s,\lambda)=f(x)-\lambda^T(h(x)-b)-\lambda^Ts
$$
with $s\geq 0$, subject to $\lambda \in \Lambda$ the [[Feasible Lagrange Multipliers]]
(where $s$ represents the slack variables)

Now suppose $\lambda_{i}>0$ for some $i$.
Then $\lim_{s_{i}\to \infty}L=-\infty$ and thus $\lambda \not\in \Lambda$.

Hence we have to have $\lambda\leq0$. 
But then $-\lambda^{T}s\geq 0$  
As $s$ is freely chosen, we have to have $\lambda^{T}s=0$
so either $\lambda_i=0$ or $s_i=0$ for any $i$.
This is called complimentary slackness.
