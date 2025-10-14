The number $\genfrac{ \{ } {\} }{0pt}{0}{ n }{ k }$ (read $n$ partition $k$) 
is the number of partitions of $[n]$ into $k$ parts, 
or equivalently, 
the number of equivalence relations of $[n]$
with $k$ equivalence classes

### Theorem
$$
\genfrac{ \{ }{ \} }{0pt}{0}{ n+1 }{ k } = \genfrac{ \{ }{ \} }{0pt}{0}{ n }{ k-1 } + k \genfrac{ \{ }{ \} }{0pt}{0}{ n }{ k }
$$
#### Proof
We have two cases.
If $\{ n+1 \}$ is an equivalence class, 
then there is $k-1$ other equivalence classes in $[n]$
This gives $\genfrac{ \{ }{ \} }{0pt}{0}{ n }{ k-1 }$.
Alternatively, if $n+1$ is in some other equivalence class,
then there were $\genfrac{ \{ }{ \} }{0pt}{0}{ n }{ k }$ ways to choose the other equiv classes,
and $k$ ways to add $n+1$ to one of them.
### Theorem
$$
x^{n} = \sum_{k=0}^{n} \genfrac{ \{ }{ \} }{0pt}{0}{ n }{ k } x^{\underline{k}}
$$
#### Proof

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
#### Proof
We use prev theorem to change basis of the vector space $V$ 
of polynomials of degree $\leq n$ from $\{ 1,x,x^{2},\dots,x^{n} \}$ to 
$$
\left\{ \binom{ x }{ 0 }, \binom{ x }{ 1 }, \dots, \binom{ x }{ n } \right\}
$$
Now just calculate:
$$
P_{n}(m) = \sum_{x=1}^{m} x^{n} = \sum_{x=1}^{m} \sum_{k=0}^{n}  \genfrac{ \{ }{ \} }{0pt}{0}{ n }{ k } x^{\underline{k}} = \sum_{k=0}^{n} k! \genfrac{ \{ }{ \} }{0pt}{0}{ n }{ k } \sum_{x=1}^{m} \binom{ x }{ k }
$$
