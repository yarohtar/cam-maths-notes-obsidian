Given integers $n,k$ with $0\leq k\leq n$
the binomial coefficient ${n \choose k}$ 
is the number of $k$ element subsets of $[n]=\{ 1,2,\dots,n \}$
where by convention $\binom{0}{0}= 1$

For $\mathbb{F}$ a [[Field]] containing $\mathbb{Q}$,
define 
$$
\binom{ \alpha }{ k } = \frac{ \alpha^{\underline{k}} }{ k! }
$$
using [[Falling Factorial]]

### Theorem
$$
\binom{ \alpha+1 }{ k } = \binom{ \alpha }{ k } + \binom{ \alpha }{ k-1 }
$$
for all $\alpha \in \mathbb{F}$
### Theorem
$$
\binom{ n }{ k } = \frac{ n(n-1)\dots(n-k+1) }{ k(k-1)\dots 1 } = \frac{n!}{k!(n-k)!}
$$
### Theorem
$$
\sum_{k=0}^{n}\binom{ n }{ k }x^{k}y^{n-k}=(x+y)^{n}
$$
### Corollary
$$
\sum_{k=0}^{n} \binom{ n }{ k } = 2^{n}
$$
$$
\sum_{k=0}^{n} \binom{ n }{ k }(-1)^{k}=0
$$
### Theorem
$$
\sum_{m=k}^{n} \binom{ m }{ k } = \binom{ n+1 }{ k+1 }
$$
