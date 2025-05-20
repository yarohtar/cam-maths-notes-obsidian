Suppose we have a numerical scheme 
$$
u'=Au
$$
for some matrix $A$.
Often, $A$ is naturally represented as $A=B+C$.
In [[Numerical Schemes as Approximations to Exp]],
we want to find $e^{tA}=e^{t(B+C)}$
Using [[Product of matrix exponentials]]:
$$
e^{tA} = e^{tB}e^{tC} + \frac{1}{2} t^{2}(CB-BC)+O(t^{3})
$$
and if $B$ and $C$ commute:
$$
e^{tA}=e^{tB}e^{tC}
$$
### Example
Suppose we are solving the diffusion equation 
$$
u_{t}=u_{x x}+ u_{y y}
$$
Using the 5-point method, we get:
$$
u_{t}=\frac{1}{h^{2}}(A_{x}+A_{y})u
$$
We can show that $A_{x}=G\otimes I$ and $A_{y}=I\otimes G$ 
where $\otimes$ is [[Kronecker Product]].
Then $A_{x}A_{y}=A_{y}A_{x}=G\otimes G$, so they commute.
We can write the following numerical scheme:
$$
u^{n+1}=e^{k(A_{x}+A_{y})/h^{2}}u^n=e^{kA_{x}/h^{2}}e^{kA_{y}/h^{2}}u^n
$$
Split Crank-Nicolson now uses
$$
r(z)=\left( 1+\frac{z}{2} \right)\left( 1-\frac{z}{2} \right)^{-1}
$$
to approximate the exponential
$$
u^{n+1} = \left( I+ \frac{\mu}{2}A_{x} \right)\left( I- \frac{\mu}{2}A_{x} \right)^{-1}\left( I+ \frac{\mu}{2}A_{y} \right)\left( I- \frac{\mu}{2} A_{y} \right)^{-1} u^{n}
$$
where the inverse is calculated in $O(M^2)$ due to its nice structure (block diagonal with tridiagonal blocks). Note that in $A_{x}$ we first need to appropriately permute the rows and columns to make it nice.
The stability is verified:
$$
\lVert r(\mu A_{x})r(\mu A_{y}) \rVert \leq \lVert r(\mu A_{x}) \rVert \lVert r(\mu A_{y}) \rVert \leq 1
$$


### Inhomogeneous case
The above works for zero boundary conditions. If that was not the case, we would have something like:
$$
u'=Au+b
$$
where $b(t)$ originates from the boundary conditions.
The exact solution for this is:
$$
u(t)=e^{tA}u(0)+\int_{0}^te^{(t-s)A}b(s)ds
$$
we can approximate this by:
$$
u^{n+1}=e^{kA}u^{n}+\frac{1}{2}k[e^{kA}b(t_{n})+b(t_{n+1})]
$$
and then use the splitting.