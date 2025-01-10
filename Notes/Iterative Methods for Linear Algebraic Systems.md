We want to find numerical solutions to
$$
Ax=b
$$
with a rule $x^{k+1}=f_{k}(x^{0},x^{1},\dots,x^{k})$
We consider linear, one step, stationary schemes:
$$
x^{k+1}=Hx^{k}+v
$$
We choose $H$ and $v$ such that an exact solution $x^{*}$ satisfies 
$$x^{*}=Hx^*+v$$
Standard terminology:
- $H$ is the iteration matrix
- $e^k=x^*-x^k$ is the error
- $r^k=Ae^k=b-Ax^k$ is the residual

We want the method to converge for any starting value of $x_{0}$.
So we want $e^k\to 0$ for any $e^0$
So we want $H^ke^0\to 0$ for any $e^0 \in \mathbb{R}^n$
So we want $\rho(H)<1$.

### Iterative refinement
By writing
$$
x^{k+1}=x^{k}-S(Ax^{k}-b)
$$
we see that $S=A^{-1}$ immediately solves the equation. So we want to find $S$ which approximates $A^{-1}$. This will give an iteration matrix $H_{S}=I-SA$.

### Splitting
Take now:
$$
(A-B)x^{k+1}=-Bx^{k}+b
$$
with the iteration matrix $H=-(A-B)^{-1}B=I-(A-B)^{-1}A$
So we want to approximate $A^{-1}$ with $(A-B)^{-1}$.

[[Jacobi Method]]
[[Gauss-Seidel Method]]

[[The Householder-John]]