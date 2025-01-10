[[Iterative Methods for Linear Algebraic Systems]]

Let $A=L_{0}+D+U_{0}$ where they are respectively: lower triangle, diagonal and upper triangle. 
We take $A-B=L_{0}+D$
We obtain the next iteration by solving:
$$
(L_{0}+D)x^{k+1}=-U_{0}x^k+b
$$
So $H_{GS}=-(L_{0}+U)^{-1}U_{0}$

Note that there is no need to calculate the inverse explicitly, because we can calculate the components of $x^{k+1}$ by forward substitution.
### Theorem
If $A$ is [[Strictly diagonally dominant]], then the Gauss-Seidel converges.
#### Proof
Lecture 17