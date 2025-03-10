A generator polynomial $g(X)$ for a [[Cyclic Code]] $C$ is a polynomial $g(X)\mid X^{n}-1$ such that
$$
\mathcal{C}=\{ f(X)g(X) \mid f(X)\in \mathbb{F}_{2}[X] \}
$$
### Theorem
Every [[Cyclic Code]] has a generator polynomial.
### Properties
If [[Cyclic Code|cyclic codes]] $C_{1}$ and $C_{2}$ have generator polynomials $g_{1}$ and $g_{2}$ then $C_{1}\supseteq C_{2}\iff g_{1}\mid g_{2}$
Also, if $N$ is odd, $f(X)=X^{N}-1$ has no repeated roots so
$X^{N}-1=f_{1}(X)\dots f_{k}(X)$ where $f_{1},\dots,f_{k}$ are distinct irreducible polynomials in $\mathbb{F}_{2}[X]$ 
So number of cyclic codes of length $N$ is $2^{k}$

### Lemma
Let $C$ be a [[Cyclic Code]] of length $n$ with generator polynomial
$g(X)=a_{0}+a_{1}X+\dots+a_{k}X^{k}$ (where $a_{k}\neq 0$)
