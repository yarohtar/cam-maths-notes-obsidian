Given a number $N$, find a nontrivial factor.

We try to use [[Periodicity Determination]] on a function $f(x)=a^{x}\pmod{N}$ finding some smallest period $r$.
If $r$ is even, we find that 
$$
N\mid a^{r}-1=(a^{r/2}-1)(a^{r/2}+1)
$$
As $r$ is the smallest period, it cannot be that $N\mid a^{r/2}-1$. 
Now 