Let $n$ be an odd integer and let $r\geq 1$ such that $2^{r}\equiv 1 \pmod{n}$. 
Let $K\simeq \mathbb{F}_{2^{r}}$ be a [[Finite Field]]
Define $\mu_{n}(K)=\{ x\in K:x^{n}=1 \}\leq K^{\times}$
Note that $n\mid 2^{r}-1$ so this subgroup has $n$ elements. 
As $K^{\times}$ is cyclic, so is $\mu_{n}(K)$ so 
$$
\mu_{n}(K)=\{ 1,\alpha,\alpha^{2},\dots,a^{n-1} \}
$$
The [[Cyclic Code]] of length $n$ with defining set $A\subseteq \mu_{n}(K)$ is the code:
$$
C=\{ f(X)\in \mathbb{F}_{2}[X] /(X^{n}-1): (\forall a\in A)\ f(a)=0 \}
$$
Note that here we say $f(a)=0$ in $K\simeq \mathbb{F}_{2^{r}}$ rather than $\mathbb{F}_{2} /(X^{n}-1)$.
### Example
$n=7$, $r=3$
$K\simeq \mathbb{F}_{8}\simeq \mathbb{F}_{2}[X] /g(X)$ for some irreducible $g$ of degree 3.
