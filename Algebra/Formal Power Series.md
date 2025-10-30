Let $R$ be a [[Algebra/Ring Theory/Ring|Ring]].
We define $R[[x]]$ to be the ring of power series, with elements
$$
a(x) = a_{0} + a_{1}x + a_{2} x^{2} + \dots
$$
for any sequence $a_{0},a_{1},\dots \in R$
and with operations defined as:
$$
f(x)+g(x) = (f_{0}+g_{0}) + (f_{1}+g_{1})x + \dots
$$
$$
f(x)\cdot g(x) = \sum_{n\geq 0} \left(\sum_{i=0}^{n} f_{i}g_{n-i} \right) x^{n}
$$
where $\sum_{n\geq 0}$ should be viewed as just a shorthand, and not an actual sum.

We will write $[x^{n}]a$ to mean $a_{n}$ when $a(x)=a_{0}+a_{1}x+\dots$
We also define $\deg a=n$ for the smallest $n\geq 0$ such that $a_{n}\neq0$.

[[Series in a Ring]]
[[Formal Infinite Sum]]
[[Formal Infinite Product]]
[[Formal Composition]]
[[Formal Derivative]]
[[Formal Maclaurin]]
[[Formal Exponential]]
[[Formal Logarithm]]
[[Formal Binomial Power]]
[[Formal Binomial Theorem]]
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

