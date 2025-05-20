We consider 
$$
u_{t}=u_{x}
$$
for $t\geq 0$ and $x\in \mathbb{R}$
with initial condition $u(x,0)=\phi(x)$.
Note that this has exact solution $u(x,t)=\phi(x+t)$

### Downward instability
Consider the [[Semidiscretization]]:
$$
\frac{\partial u_{m}(t)}{\partial t} = \frac{1}{2h} (u_{m}(t)-u_{m-1}(t))
$$
using the [[Euler method]]:
$$
u_{m}^{n+1}=u_{m}^{n}+m
$$