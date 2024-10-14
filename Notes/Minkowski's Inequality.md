### Lemma
$f(x)=x^p$ is convex for $1\leq p<\infty$
#### Proof
Need to show $$
(\lambda x+(1-\lambda)y)^p\geq \lambda x^p +(1-\lambda)y^p
$$ WLOG $x\leq y$. It is certainly true for $x=y$ (then inequality holds). Now take derivative and show LHS>RHS.

### Minkowski's Inequality
Let $1\leq p<\infty$ and $x,y\in L_{p}$. Then $x+y\in L_{p}$ and $||x+y||_{p}\leq ||x||_{p}+||y||_{p}$.
#### Proof
First show if $||x||_{p}, ||y||_{p}\leq 1$ then $||\lambda x+(1-\lambda)y||_{p}\leq 1$ for all $0<\lambda<1$. 
For each $n$ have $|\lambda x_{n}+(1-\lambda)y_{n}|^p\leq \lambda|x_{n}|^p+(1-\lambda)|y_{n}|^p$ (using lem)