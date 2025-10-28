$$
\exp(x) = \sum_{n\geq 0} \frac{ x^{n} }{ n! }
$$
### Theorem
$$
\exp\left( \sum_{n=1}^{\infty} A_{n}(x) \right) = \prod_{n=1}^{\infty} \exp(A_{n}(x))
$$
so long as $\deg(A_{n})\geq 1$ and $\deg(A_{n})\to \infty$ as $n\to \infty$.
#### Proof
Prove by induction for finite sums. 
Then the coefficient of $x^{m}$ is unaffected by $A_{n}(x)$ for $n>m$
so we have equality in the infinite sum also.
