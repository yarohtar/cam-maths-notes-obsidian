Let $T$ be the [[Combinatorial Structure]] of [[Tree]]s.
Let $f(x)=\tilde{f}_{T_{\bullet}}(x)$ be the [[Exponential Generating Function]] for rooted trees.
Let $g(x)=\tilde{f}_{(T_{\bullet})_{\bullet}}(x)$ be the [[Exponential Generating Function]] for doubly rooted trees.
### Lemma
$$
f(x) = xe^{f(x)}
$$
#### Proof
Note that 
$$
T_{\bullet} = X \times \mathrm{Set}(T_{\bullet})
$$
as we can pick one vertex $r$ to be the root;
then build rooted trees on other vertices;
and finally connect $r$ to the roots of the trees in $\mathrm{Set}(T_{\bullet})$.
As $f_{\mathrm{Set}}=\exp$ we conclude 
$$
f(x) = x \exp(f(x))
$$
### Lemma
$$
g(x) = f(x) + f(x)^{2} + \dots
$$
In addition 
Let $\mathcal{A}=(\{ f:[n]\to[n] \},1)$. Then $\tilde{f}_{\mathcal{A}}(x) =g(x)$
#### Proof
For any $k\geq 1$, build the [[Combinatorial Product]]
$$
\underbrace{T_{\bullet}\times\dots \times T_{\bullet}}_{k\text{ times}}
$$
and then connect their roots in order.
We now view just the endpoints as being the roots.
Also, in any doubly rooted tree, 
the distance between the two roots is some $k\geq 1$ (edges).
Thus we conclude 
$$
g(x) = f(x) + f(x) ^{2} + \dots
$$

Any $f:[n]\to[n]$ must have $k$ periods and $(2k)$ wandering points for some $k\geq 1$.
There is a bijection between $\{ f:[n]\to[n] \}$ 
with $k$ periodic points and unordered partitions of $[n]$
into $k$ parts on each of which I build a rooted trees cartesian product the permutations $f$ define on these $k$ paths .......... uh something....


### Theorem
There are $n^{n-2}$ spanning trees on $[n]$.