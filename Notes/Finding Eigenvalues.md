[[Power Method for Finding Eigenvalues]]
[[Inverse Iteration for Finding Eigenvalues]]
## Deflation
Given an eigenvalue $\lambda$ with eigenvector $w$ of $A$, 
we want to deflate $A$ to a smaller matrix and find the next eval.
Use a [[Householder Reflection]] 
$$
H_{u} = I - 2\frac{uu^{T}}{\lVert u \rVert ^{2}}
$$
with $u=w$