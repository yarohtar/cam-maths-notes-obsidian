The number $\genfrac{ \{ } {\} }{0pt}{0}{ n }{ k }$ (read $n$ partition $k$) 
is the number of partitions of $[n]$ into $k$ parts, 
or equivalently, 
the number of equivalence relations of $[n]$
with $k$ equivalence classes

$$
\genfrac{ \{ }{ \} }{0pt}{0}{a}{b}
$$
### Theorem
$$
\genfrac{ \{ }{ \} }{0pt}{0}{ n+1 }{ k } = \genfrac{ \{ }{ \} }{0pt}{0}{ n }{ k-1 } + k \genfrac{ \{ }{ \} }{0pt}{0}{ n }{ k }
$$
### Theorem
$$
x^{n} = \sum_{k=0}^{n} \genfrac{ \{ }{ \} }{0pt}{0}{ n }{ k } x^{\underline{k}}
$$
### Theorem
$$
x^{n} = \sum_{k=0}^{n}(-1)^{n-k} x^{\overline{k}}
$$
### Theorem
Given $n,m\in \mathbb{N}$, want to find
$$
P_{n}(m) = 1^{n} + 2^{n} + \dots + m^{n} 
$$
is a polynomial of degree $n+1$ given by
$$
P_{n}(m) = \sum_{k=0}^{n} k! \genfrac{ \{ }{ \} }{0pt}{0}{ n }{ k } \binom{ m+1 }{ k+1 }
$$
We use prev theorem to change basis of the vector space $V$ 
of polynomials of degree $\leq n$ from $\{ 1,x,x^{2},\dots,x^{n} \}$ to 
$$
\left\{ \binom{ x }{ 0 }, \binom{ x }{ 1 }, \dots, \binom{ x }{ n } \right\}
$$
$$
P_{n}(m) = \sum_{x=1}^{m} x^{n} = \sum_{x=1}^{m} \sum_{k=0}^{n}  \genfrac{ \{ }{ \} }{0pt}{0}{ n }{ k } x^{\underline{k}} = \sum_{k=0}^{n} k! \genfrac{ \{ }{ \} }{0pt}{0}{ n }{ k } \sum_{x=1}^{m} \binom{ x }{ k }
$$
