[[Iterative Methods for Linear Algebraic Systems]]
[[Exact Line Search]]
### Theorem
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
For $k\geq 0$ find $x^{}$
