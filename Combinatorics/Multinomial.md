There are 
$$
\binom{ n+k-1 }{ k-1 }
$$
$k$-partitions of $n$, i.e. integer $k$-tuples $(a_{1},\dots,a_{k})$ s.t. $n=a_{1}+\dots+a_{k}$
The number 
$$
\binom{ n }{ a_{1},\dots,a_{k} }
$$
of partitions of $[n]$ into sets of size $a_{1},\dots,a_{k}$ is called the multinomial.

### Theorem
$$
\binom{ n }{ a_{1},\dots,a_{k} } = \frac{ n! }{ a_{1}! \dots a_{k}! }
$$
### Theorem
$$
\sum_{n=a_{1}+\dots+a_{k}} \binom{ n }{ a_{1},\dots,a_{k} } x_{1}^{a_{1}}\dots x_{k}^{a_{k}} = (x_{1}+\dots+x_{k})^{n} 
$$
#### Proof
Count the set $S_{n}$ of permutations of $[n]$ in two ways.
Firstly
$$
\lvert S_{n} \rvert = n!
$$
Define equivalence relation $\sim$ on $\sigma \in S_{n}$
by $\sigma \sim \sigma'$
if and only if
$\sigma, \sigma'$ permute each other on consecutive blocks of size $a_{1},\dots,a_{k}$
Thus find:
$$
\lvert S_{n} / \sim \rvert = \binom{ n }{ a_{1},\dots,a_{k} }
$$
and each equivalence class has size $a_{1}!a_{2}!\dots a_{k}!$

The multinomial expansion follows ...