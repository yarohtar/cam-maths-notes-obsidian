[[Iterative Methods for Linear Algebraic Systems]]
Let $A=L_{0}+D+U_{0}$ where they are respectively: lower triangle, diagonal and upper triangle. 
Set $A-B=D$
We obtain the next iteration by solving
$$
Dx^{k+1}=-(L_{0}+U_{0})x^{k}+b
$$
so $H_{J}=-D^{-1}(L_{0}+U_{0})$

### Theorem
If $A$ is [[Strictly diagonally dominant]], then the Jacobi method converges.
#### Proof
Lecture 17

### Theorem
If both $A$ and $2D-A$ are symmetric positive definite, then Jacobi method converges
#### Proof
Use [[The Householder-John Theorem]].