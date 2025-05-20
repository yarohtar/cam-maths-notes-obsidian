We consider the equation:
$$
\frac{\partial u}{\partial t}= \frac{\partial u}{\partial x}
$$
for $0\leq x\leq 1$ and $t\geq 0$
with initial conditions $u(x,0)=u_{0}(x)$ for $t=0$
and Dirichlet boundary conditions $u(0,t)=\phi_{0}(t)$ at $x=0$
and $u(1,t)=\phi_{1}(t)$ at $x=1$


## Crank-Nicolson method
[[Crank-Nicolson method]]
We use [[Semidiscretization]]:
$$
\frac{du_{m}}{dt} = \frac{1}{2h} (u_{m+1} - u_{m-1})
$$
and [[Trapezoidal rule (ODEs)]]
$$
u_{m}^{n+1}-u_{m}^{n}=\frac{1}{4} \mu(u_{m+1}^{n+1}-u_{m-1}^{n+1}) + \frac{1}{4}\mu(u_{m+1}^{n}-u_{m-1}^{n})
$$
### Lemma
This is stable for all $\mu>0$.
#### Proof
We find $u^{n+1}=B^{-1}Cu^{n}$ 
where $B$ and $C$ are [[TAntiST Matrix]] and hence [[Normal Matrix]]
$$
B=\begin{pmatrix}
1 & -\frac{1}{4}\mu &  \\
\frac{1}{4}\mu & 1 & \ddots &  \\
 & \ddots & \ddots & -\frac{1}{4}\mu \\
 &  & \frac{1}{4}\mu & 1 
\end{pmatrix}
\quad %quad
C=\begin{pmatrix}
1 & \frac{1}{4}\mu &  \\
-\frac{1}{4}\mu & 1 & \ddots &  \\
 & \ddots & \ddots & \frac{1}{4}\mu \\
 &  & -\frac{1}{4}\mu & 1
\end{pmatrix}
$$
Then $A=B^{-1}C$ shares its eigenvectors with $B$ and $C$ so:
$$
\lambda_{k}(A)=\frac{\lambda_{k}(C)}{\lambda_{k}(B)} = \frac{1+\frac{1}{2}i\mu \cos kx}{1-\frac{1}{2}\mu \cos kx}
$$
$$
\lvert \lambda_{k}(A) \rvert =1
$$
$A$ is also [[Normal Matrix]] so $\rho(A)=1$, thus the method is stable.
