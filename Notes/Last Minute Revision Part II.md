# LST
## Mostovski
## $\kappa^{2}=\kappa$
# Numerical
[[Numerical Analysis]]
## Householder-John
Let $A$ and $B$ are real matrices such that 
both $A$ and $A-B-B^T$ are symmetric positive definite.
Define $H=-(A-B)^{-1}B$.
Then $\rho(H) < 1$
### Proof
Key point is, for complex $w$ and positive definite $C$ it still holds:
$$
w^{\dagger}Cw>0
$$
Then just apply this to $A-B-B^{T}$ and do some algebra
## 
# Asymptotic
## $\Gamma$ function
![[The Gamma Function]]

## Laplace Method
### The method
### Integrals
$$
\int_{0}^{\infty} u^{n} e^{-Au^{p}} du = \frac{A^{-(n+1)/p}}{p} \Gamma\left( \frac{n+1}{p} \right)
$$
$$
\int_{-\infty}^{\infty} u^{2m} e^{-Au^{2q}} du = \frac{A^{-(2m+1)/(2q)}}{q} \Gamma\left( \frac{2m+1}{2q} \right)
$$
$$
\int_{-\infty}^{\infty} u^{2m+1} e^{-Au^{2q}}du = 0
$$ 
# Numerical Analysis