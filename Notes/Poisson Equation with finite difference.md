We want to solve:$$
\nabla^2u = f
$$
subject to some Dirichlet boundary conditions. For this method we will assume that the boundary is rectangular because finite difference gets a bit messed up otherwise.

We use [[Finite difference|finite differences]] to discretize the equation. 
$$
\Delta_{h,x}^2u+\Delta_{h,y}^2u=h^2f(x,y)
$$
ie we get
$$
u(x-h,y)+u(x+h,y)+u(x,y-h)+u(x,y+h)-4u(x,y)=h^2f(x,y)
$$
Now let $u_{i,j}=u(ih,jh)$ and $f_{i,j}=f(ih,jh)$ to get
$$
u_{i-1,j}+u_{i+1,j}+u_{i,j-1}+u_{i,j+1}-4u_{i,j}=h^2f_{i,j}
$$
Now we make $u$ into a column vector, and rewrite the system of equations into $Au=b$ (note that $u_{0,j}$ and $u_{i,0}$ are boundary conditions and should be on rhs). If we fill the column vector $u$ in a natural way (column by column in the grid) then the matrix $A$ looks like this (in block matrix format):
$$
A=\begin{pmatrix} 
B & I  \\
I & B & I \\
 & I & B & \ddots  \\
 &  & \ddots & \ddots & I  \\
& & & I & B
\end{pmatrix}
$$
$$
B=
\begin{pmatrix}
-4 & 1  \\
1 & -4 & 1 \\
 & 1 & -4 & \ddots \\
& & \ddots & \ddots & 1 \\
& & & 1 & -4
\end{pmatrix}
$$
We investigate this matrix, and try to prove that this discrete version does converge to the actual solution when $h$ is small.
[[Gershgorin Theorem]]
## Lemma
For any ordering of the grid points, the matrix $A$ is symmetric and negative definite.
### Proof
Firstly note that $a_{ii}=-4$ for all $i$.
Now for $i\neq j$, if $u_{i}$ and $u_{j}$ are neighbours then $a_{ij}=a_{ji}=1$, otherwise $a_{ij}=a_{ji}=0$, so $A$ is symmetric and has real eigenvalues.
Now by [[Gershgorin Theorem]] the eigen values are at most $0$ (each row will have at most 4 entries that are $1$). Suppose now we have an eigenvalue 0 with eigenvector $x$. Let $i$ be the index st $x_i$ is the max absolute component of $x$. Then $x_j$ has to have the same modulus whenever $a_{ij}=1$. But then we can change $i$ to one of these and expand all the way to the boundary where we will get a contradiction.

### Proposition
The eigenvalues of $A$ are 
$$
\lambda_{k,l}=-4\left( \sin^2 \frac{k\pi h}{2}+ \sin^2 \frac{l\pi h}{2} \right)
$$
where $h=\frac{1}{m+1}$ and $k,l=1,\dots,m$

#### Proof
Fix $k$ and $l$ and we define $x=k\pi h$ and $y=l\pi h$. We prove that $$
v_{i,j}=\sin ix \sin jy
$$ is an eigenvector. We do some CURSED rearranging and it works.


### Theorem
This converges.
#### Proof
$$
e_{i-1,j}+e_{i+1,j}+e_{i,j-1}+e_{i,j+1}-4e_{i,j}=h^2f_{i,j}+\nu_{i,j}
$$
$$
Ae=\nu\implies e=A^{-1}\nu\implies ||e||\leq ||A^{-1}||\cdot||\nu||
$$
$$
||\nu ||^2=\sum_{i=1}^{m} \sum_{j=1}^{m} |\nu_{i,j}|^2\leq c^2m^2h^8<c^2 \frac{1}{h^2}h^8=c^2h^6
$$ $$
\implies ||\nu||\leq ch^3
$$
The eigenvalues of $A^{-1}$ are the inverses of eigenvalues of $A$ - but we know those. 
$$
||A^{-1}||=\frac{1}{4} \max \{ (\sin^2+\sin^2)^{-1} \} \leq \frac{1}{8\sin^2\left( \frac{\pi h}{2} \right)}\leq \frac{1}{8h^2}
$$
So finally 
$$
||e||\leq ||A^{-1}||\cdot||\nu||\leq \frac{ch}{8}
$$


