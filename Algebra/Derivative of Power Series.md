Given a [[Formal Power Series]]
$$
A(x) = \sum_{n\geq 0} a_{n} x^{n}
$$
define the derivative 
$$
A'(x) = \sum_{n\geq 0} (n+1) a_{n+1} x^{n}
$$
### Remark
Think of it as building a structure on $n+1$ elements 
and then choosing one of those elements to be special (in $n+1$ ways).
### Lemma
$$
(A(x)+B(x))'=A'(x)+B'(x)
$$
$$
(A(x)\cdot B(x))' = A(x)B'(x) + A'(x)B(x)
$$
$$
(B(x)^{n})' = n(B(x)^{n-1})B'(x)
$$
$$
B(A(x)) = A'(x) B'(A(x))
$$
### Theorem
$$
A(x) = \sum_{n\geq 0} a_{n}x^{n} = \sum_{n\geq 0} \frac{ A^{(n)}(0) }{ n! } x^{n}
$$
### Defn
$$
\exp(x) = \sum_{n\geq 0} \frac{ x^{n} }{ n! }
$$
$$
-\log(1-x) = \sum_{n\geq 0} \frac{ x^{n} }{ n }
$$
$$
(1+x)^{r} = \exp(r\log(1+x))
$$
for $r\in R$
### Remark
$$
(\exp x)' = \exp x
$$
$$
(-\log(1-x))'= \frac{1}{1-x}
$$
$$
\exp(\log(1+x)) = 1+x
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

