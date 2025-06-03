[[Iterative Methods for Linear Algebraic Systems]]
[[Exact Line Search]]
## Theorem
Let $d^{0},d^{1},\dots,d^{n-1}$ be $n$ [[Conjugate Directions]]
and consider the sequence of iterates:
$$
x^{k+1}= x^{k} + \alpha_{k} d^{k}
$$
where 
$$
\alpha_{k} = \frac{(r^{k},d^{k})}{(d^{k},Ad^{k})}
$$
Then $r^{k}$ is orthogonal to $d^{0},\dots,d^{k-1}$.
In particular $r^{n}=0$.
#### Proof
Nothing special, just check.

# The method
### Initial conditions
For any initial $x^{0}$, set $d^{0}=r^{0}=b-Ax^{0}$
### Iterate
For $k\geq 0$ find $x^{k+1}$ and $r^{k+1}$ by the usual formula (above)
### Next direction
The next conjugate direction is:
$$
d^{k+1} = r^{k+1} +\beta_{k} d^{k}
$$
with
$$
\beta_{k} = - \frac{(r^{k+1},Ad^{k})}{(d^{k},Ad^{k})}
$$
i.e. the value that makes $d^{k+1}$ normal to $Ad^{k}$
## Theorem (properties)
For every $m\geq 0$, the conjugate gradient satisfies:
1. $\operatorname{span}\{ r_{i} : i<k\}=\operatorname{span}\{ d_{i} : i<k\}$ for every $k$