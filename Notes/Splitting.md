Suppose we are solving the diffusion equation 
$$
u_{t}=u_{x x}+ u_{y y}
$$
Using the 5-point method, we get:
$$
u_{t}=\frac{1}{h^{2}}(A_{x}+A_{y})u
$$
Now as $A_{x}$ and $A_{y}$ commute, using [[Product of matrix exponentials]] we can write the following numerical scheme:
$$
u^{n+1}=e^{k(A_{x}+A_{y})/h^{2}}u^n=e^{kA_{x}/h^{2}}e^{kA_{y}/h^{2}}u^n
$$
Split Crank-Nicolson now uses
$$
r(z)=\left( 1+\frac{z}{2} \right)\left( 1-\frac{z}{2} \right)^{-1}
$$
to approximate the exponential.
where the inverse is calculated in $O(M^2)$ due to its nice structure (block diagonal with tridiagonal blocks) 
