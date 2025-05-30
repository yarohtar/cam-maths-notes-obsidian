# LST
## Mostovski
## $\kappa^{2}=\kappa$
# Numerical analysis
[[Numerical Analysis]]
## PDEs
### Finite difference
$$
\frac{1}{h^2}[g(x-h)-2g(x)+g(x+h)]=g''(x)+\frac{1}{12}h^2g^{(4)}(x)+\frac{1}{360}h^4g^{(6)}(x)+O(h^6)
$$

## Iterative methods
### Gauss-Scheidel
![[Gauss-Seidel Method]]
### Jacobi
![[Jacobi Method]]
### Householder-John
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
### That last thing that I never typed out
# Asymptotic
## $\Gamma$ function
![[The Gamma Function]]

## Watson's lemma
[[Watson's lemma]]
## Laplace Method
[[Laplace Method]]
$$
F(x) = \int_{a}^{b} f(t)e^{x\phi(t)} dt
$$
### The method
1. Draw picture
2. Find GLOBAL maxima
3. Around each max, write a taylor expansion
$$
x\phi(t) \sim x\phi(c) + xA_{p}(t-c)^{p} + xA_{p+1}(t-c)^{p+1} + \dots
$$
4. Use substitution $t=c+x^{-1/p}u$
5. Use integrals below
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