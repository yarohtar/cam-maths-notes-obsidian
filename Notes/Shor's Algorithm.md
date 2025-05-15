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
