[[Threshold Scheme]]
### Shamir's method
Let $0\leq S\leq N$ be the secret which can be chosen at random 
by the Leader.
The Leader chooses a prime $p>n,N$.
The Leader chooses independent random coefficients
$a_{1},\dots,a_{k-1}$ with $0\leq a_{j}\leq p-1$ where $a_{0}=S$,
and distinct integers $x_{1},\dots,x_{n}$ with $1\leq x_{j}\leq p-1$
Define:
$$
P(r)=a_{0}+\sum_{j=1}^{k-1}a_{j}x_{r}^{j}\pmod{p}
$$
