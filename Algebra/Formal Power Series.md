Let $R$ be a [[Algebra/Ring Theory/Ring|Ring]].
We define $R[[X]]$ to be the ring of power series, i.e. 
$$
f(x) = a_{0} + a_{1}x + a_{2} x^{2} + \dots
$$
[[Composition of Power Series]]
[[Derivative of Power Series]]
[[Formal Binomial Theorem]]
### Infinite sum
Let 
$$
\begin{align}
A_{1}(x)  = &  a_{10} + a_{11} x + a_{12} x^{2} + \dots \\
A_{2}(x)   = &  a_{20} + a_{21}x + a_{22} x^{2} + \dots \\
A_{3}(x)   =  & a_{30} + a_{31}x + a_{32}x^{2} + \dots  \\
 & \vdots
\end{align}
$$
be an infinite family of powerseries in $R[[X]]$
Then the sum
$$
\sum_{n=0}^{\infty} A_{n}
$$
is well defined iff for any $j\geq 0$
the column sum 
$$
\sum_{i=1}^{\infty} a_{ij}
$$
is a finite sum so the difference with $S_{N}(x) = \sum_{n=1}^{N}A_{n}(x)$
has degree $r$ i.e. smallest integer such that $[x^{m}]$ is non-zero tending to $\infty$

### Theorem
Let $a_{n}$ be the number of ways to build a certain structure $\mathcal{A}$
on an $n$-element set, 
and let $b_{n}$ be the number of ways to build another structure $\mathcal{B}$ 
on an $n$-element set.
Then let $c_{n}$ be the number of ways to separate $[n]$ into disjoint intervals $S\cup T$
where $S=\{ 1,2,\dots,i \}$ and $T=\{ i+1,\dots,n \}$ and build $\mathcal{A}$ on $S$ and $\mathcal{B}$ on $T$.
Then 
$$
C(x) = \sum_{n\geq 0} c_{n}x^{n} = A(x) B(x)
$$
We call this structure $\mathcal{A}\cdot \mathcal{B}$.
### Theorem
For disjoint union $\mathcal{A}\sqcup \mathcal{B}$ we have $A(x)+B(x)$. 
### Theorem
Suppose $a_{0}=0$.
Let $h_{n}$ be the number of ways to split $[n]$ into disjoint nonempty intervals 
and build structure $\mathcal{A}$ on each. Also let $h_{0}=1$.
Then 
$$
H(x)=\sum h_{n} x^{n} = \frac{1}{1-A(x)}
$$
We call this $A^{*}$.
### Theorem
Suppose $a_{0}=0$ and $b_{0}=1$.
Let $g_{n}$ be the number of ways to split $[n]$ into disjoint nonempty intervals
and build $\mathcal{A}$ in each interval and $\mathcal{B}$ on the set of intervals and set $g_{0}=1$.
Then
$$
G(x)=\sum_{n\geq 0} g_{n}x^{n} = B(A(x))
$$

