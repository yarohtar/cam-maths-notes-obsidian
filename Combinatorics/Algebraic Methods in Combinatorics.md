Reading:
- Cameron (2017) Notes on counting
- Matousek (2010) 33 miniatures
- Alon (1999) Combinatorial Nullstellensatz
[[Enumerative Methods in Combinatorics]]
[[Counting in Two Ways]]
[[Weighted Graph]]
[[Adjacency Matrix]]
[[Formal Power Series]]
[[Catalan Number]]
[[Combinatorial Structure]]
[[Labelled Structure]]


### Theorem
Let $f(x)=\tilde{f}_{T_{\bullet}}(x)$ be the egf for rooted trees.
Then
$$
f(x) = xe^{f(x)}
$$
$$
g(x) = \tilde{f}_{(T_{\bullet})_{\bullet}}(x) = f(x) + f(x)^{2} + \dots
$$
Let $\mathcal{A}=(\{ f:[n]\to[n] \},1)$. Then $\tilde{f}_{\mathcal{A}}(x) =g(x)$

There are $n^{n-2}$ spanning trees on $[n]$.
#### Proof
First thing follows from
$$
T_{\bullet}=\{ \bullet \} * \mathrm{Set}(T_{\bullet})
$$
If the root-to-root path has $k$ vertices, the contribution to egf is $f(x)^{k}$ 
as it has structure the labelled product 
$$
\underbrace{ T_{\bullet}*T_{\bullet}*\dots*T_{\bullet}}_{k\text{ times}}
$$
Any $f:[n]\to[n]$ must have $k$ periods and $(2k)$ wandering points for some $k\geq 1$.
There is a bijection between $\{ f:[n]\to[n] \}$ 
with $k$ periodic points and unordered partitions of $[n]$
into $k$ parts on each of which I build a rooted trees cartesian product the permutations $f$ define on these $k$ paths 

