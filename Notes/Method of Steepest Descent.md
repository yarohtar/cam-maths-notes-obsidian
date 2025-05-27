We want to find [[Asymptotic Approximation]] of:
$$
F(x) = \int_{C} f(z) e^{x\phi(z)} dz
$$
where $C$ is a curve in $\mathbb{C}$.
The size of the integrand $e^{x\phi(z)}$ 
is determined by the real part of $\phi(z)$
Write $\phi(p+iq)=u(p,q)+iv(p,q)$
We want $u$ to be small
Path of steepest descent is the one where $u$ decreases rapidly 
So we look for the direction $-\nabla u$ i.e. curves parallel to $\nabla u$
Due to [[Cauchy-Riemann Equations]]
$$
\nabla u \cdot \nabla v = u_{p} v_{p} + u_{q} v_{q} = 0
$$
so we are looking for curves perpendicular to $\nabla v$
But these are curves of constant $v$.

Furthermore, we would like curves going through 
stationary points of $\phi$ i.e. $\phi'(z)=0$ 
The reasoning is similar to [[Laplace Method Summary]]
Note that at stationary points, we will have two possible choices
We want the one that makes the real part go to $0$
