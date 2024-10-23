Using the [[Trapezoidal rule (ODEs)]] after [[Semidiscretization]] we get:
$$
u_{m}^{n+1}-\frac{1}{2}\mu(u_{m-1}^{n+1}-2u_{m}^{n+1}+u_{m+1}^{n+1})=u_{m}^{n}+\frac{1}{2}\mu(u_{m-1}^n-2u_{m}^n+u_{m+1}^n)
$$

Define $B=I-\frac{1}{2}\mu A_{*}$ and $C=I+\frac{1}{2}\mu A_{*}$ where $A_{*}$ is a [[TST matrix]]
Let $A=B^{-1}C$.
Amazingly, $B$ and $C$ have the same set of eigenvectors, hence $A$ also does, with eigenvalues given by:
$$
\lambda_{k}(A)=\frac{\lambda_{k}(C)}{\lambda_{k}(B)}=\frac{1-2\mu \sin ^{2} \frac{1}{2}\pi kh}{1+2\mu \sin ^{2} \frac{1}{2}}
$$