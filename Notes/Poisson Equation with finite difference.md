We want to solve:
$$
\nabla^2u = f
$$
subject to some Dirichlet boundary conditions. 
## Five-point method
For this method we will assume that the boundary is rectangular because finite difference gets a bit messed up otherwise.

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
### Lemma
For any ordering of the grid points, the matrix $A$ is symmetric and negative definite.
#### Proof
Firstly note that $a_{ii}=-4$ for all $i$.
Now for $i\neq j$, if $u_{i}$ and $u_{j}$ are neighbours then $a_{ij}=a_{ji}=1$, otherwise $a_{ij}=a_{ji}=0$, so $A$ is symmetric and has real eigenvalues.
Now by [[Gershgorin Theorem]] the eigen values are at most $0$ (each row will have at most 4 entries that are $1$). Suppose now we have an eigenvalue 0 with eigenvector $x$. Let $i$ be the index st $x_i$ is the max absolute component of $x$. Then $x_j$ has to have the same modulus whenever $a_{ij}=1$. But then we can change $i$ to one of these and expand all the way to the boundary where we will get a contradiction.

### Proposition (eigenvalues)
The eigenvalues of $A$ are 
$$
\lambda_{k,l}=-4\left( \sin^2 \frac{k\pi h}{2}+ \sin^2 \frac{l\pi h}{2} \right)
$$
where $h=\frac{1}{m+1}$ and $k,l=1,\dots,m$

#### Proof
Fix $k$ and $l$ and we define $x=k\pi h$ and $y=l\pi h$. We prove that $$
v_{i,j}=\sin ix \sin jy
$$ is an eigenvector. We do some CURSED rearranging and it works.


### Theorem (convergence)
Subject to sufficient smoothness of the function $f$ and the boundary conditions $\phi$, there exists a number $c>0$, independent of $h=\frac{1}{m+1}$, such that $||e||\leq ch$.
#### Proof
Note that the exact solution satisfies our recursion relation up to an addition of some $\eta_{i,j}=O(h^{4})$. Subtracting our numerical approximation we find the recursive formula for errors:
$$
e_{i-1,j}+e_{i+1,j}+e_{i,j-1}+e_{i,j+1}-4e_{i,j}=h^2f_{i,j}+\eta_{i,j}
$$
Or in the matrix form $Ae=\eta$. Note that $A$ is invertible (nonzero eigenvalues that we found) so $e=A^{-1}\eta\implies ||e||\leq ||A^{-1}||\cdot||\eta||$
Every component of $\eta$ satisfies $|\eta_{i,j}|^2\leq c^2h^8$ for some $c$ (because $O(h^4)$), so we have:
$$
\begin{align}
||\eta ||^2&=\sum_{i=1}^{m} \sum_{j=1}^{m} |\eta_{i,j}|^2\leq c^2m^2h^8<c^2 \frac{1}{h^2}h^8=c^2h^6\\
&\implies ||\eta||\leq ch^3
\end{align}
$$
The norm of a matrix is the max modulus of an eigenvalue (because $||Ax||$ is maximal when $x$ is in the direction of the associated eigenvector)
The eigenvalues of $A^{-1}$ are the inverses of eigenvalues of $A$ - but we know those. 
$$
||A^{-1}||=\frac{1}{4} \max \{ \left(\sin^2{k\pi h\over 2}+\sin^2{l\pi h\over 2}\right)^{-1} \} \leq \frac{1}{8\sin^2\left( \frac{\pi h}{2} \right)}\leq \frac{1}{8h^2}
$$
(note in above, $\sin x\geq ax$ where $a<1$ and $x$ is small)
So finally 
$$
||e||\leq ||A^{-1}||\cdot||\eta||\leq \frac{ch}{8}
$$



## Special structure of 5 point equations
First diagnoalize $B$ with $B=QDQ^{-1}$.
Set $v_{k}=Qu_{k}$, $c_{k}=Qb_{k}$. The system becomes
$$
\begin{pmatrix}
D & I &  \\
I & D & \ddots \\
 & \ddots  & \ddots & I \\
 &  & I & D
\end{pmatrix}
v=c
$$
More reordering:
$$
\begin{pmatrix}
\Lambda_{1} & 1 \\
1 & \Lambda_{2} &  \ddots\\
 & \ddots & \ddots  & 1\\
 &  & 1 & \Lambda_{n}
\end{pmatrix}
$$
