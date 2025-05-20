Suppose we are solving the diffusion equation 
$$
u_{t}=a(x,y)u_{x x}+ b(x,y)u_{y y}
$$
### 
Using the 5-point method, we get:
$$
u_{t}=\frac{1}{h^{2}}(A_{x}+A_{y})u
$$
We can show that $A_{x}=G\otimes I$ and $A_{y}=I\otimes G$ 
where $\otimes$ is [[Kronecker Product]] and:
$$
G=\begin{pmatrix}
-2 & 1 &  \\
1 & \ddots & \ddots &  \\
 & \ddots & -2 & 1 \\
 &  & 1 & -2
\end{pmatrix}
$$
Then $A_{x}A_{y}=A_{y}A_{x}=G\otimes G$, so they commute.
Using [[Splitting Numerical Schemes]] we can write:
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
