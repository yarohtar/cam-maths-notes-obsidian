All eigenvalues of a matrix $A$ are contained in the union of Gershgorin discs in the complex plane, where a Gershgorin disc is:
$$
\Gamma_{i}=\{ z \in \mathbb{C} \mid |z-a_{ii}|\leq r_{i} \}, \quad r_{i}=\sum_{j\neq i}|a_{ij}|
$$
### Proof
Let $\lambda$ be an eigen value of $A$ with eigenvector $x$ st $Ax=\lambda x$. 
Take the largest absolute coordinate in $x$ be $i$ and divide through so that $x_{i}=1$ and $|x_{j}|\leq 1$ for $j\neq i$ (so WLOG take this $x$ at the start).
Now the $i$-th row gives 
$$
\sum_{j} a_{ij}x_{j}=\lambda
$$
Rearange to get 
$$
\lambda - a_{ii} = \sum_{j\neq i}a_{ij}x_{j}
$$
Finally, take absolute values, apply triangle ineq, and $x_j\leq 1$. 