Given a number $N$, find a nontrivial factor.

We try to use [[Periodicity Determination]] on a function $f(x)=a^{x}\pmod{N}$ finding some smallest period $r$.
If $r$ is even, we find that 
$$
N\mid a^{r}-1=(a^{r/2}-1)(a^{r/2}+1)
$$
As $r$ is the smallest period, it cannot be that $N\mid a^{r/2}-1$. 
Now $gcd(N,a^{r/2}+1)$ may give us a nontrivial factor of $N$.
This is likely to succeed. 

### Finding the period
Let $m$ be the smallest integer such that $M=2^{m}\geq N$.
Pick a random integer $2\leq a<N$.
We try to implement [[Periodicity Determination]] of $f(x)=a^{x}\pmod{N}$ on a whole domain $\mathbb{Z}_{M}$.
Start from state $\ket{0\dots 0}\ket{0}$.
Apply $H^{n}$ on the first $n$ registers:
$$
\frac{1}{\sqrt{ 2^{m} }}\sum_{x}\ket{x} \ket{0}
$$
Apply the quantum oracle $U_{f}$ for $f$:
$$
\frac{1}{\sqrt{ M }}\sum_{x}\ket{x} \ket{f(x)}
$$
We measure the last register 