Let $G$ be a [[Weighted Graph]].
Let $L_{G}$ be its [[Laplacian Matrix]].
Let $L_{G}^{*}$ be derived from $L_{G}$ by removing the $n$-th row and $n$-th column.
Consider all the spanning trees of $G$ rooted towards $n$.
The sum of all of their weights equals $\det(L_{G}^{*})$.
### Proof 1
By induction on the number of edges with nonzero weight $m$.
The case $m=0$ is trivial.
Consider the edge $e=ij$.
Let $\tau(G)$ be the combined weight of trees directed towards $n$.
Then 
$$
\tau(G) =\tau(G-e) + w(e) \tau\left(G / e \right) = \det(L_{G-e}^{*}) + w(ij) \det(L_{G / e}^{*})
$$
Note that the [[Adjacency Matrix]] of $G / e$ is formed by:
1. removing row $i$ and column $j$
2. replacing $(\mathrm{col}\ i)$ with $(\mathrm{col}\ i)+(\mathrm{col}\ j)$
3. replacing $(\mathrm{row}\ j)$ with $(\mathrm{row}\ i)+(\mathrm{row}\ j)$
Matrix $L_{G / e}^{*}$ is formed from $L_{G}^{*}$ in the same way, from where the result follows.
### Proof 2
$$
L_{G}^{*} = \begin{pmatrix}
\sum\limits_{j\neq 1} A_{1j} & -A_{12}  & \dots & -A_{1(n-1)} \\
-A_{21} & \sum\limits_{j\neq 2}A_{2j}  & \dots & -A_{2(n-1)} \\
\vdots & \vdots & \ddots & \vdots \\
-A_{(n-1)1} & -A_{(n-1)2}  & \dots & \sum \limits_{j\neq n-1}A_{(n-1)j}
\end{pmatrix}
$$
Fix a permutation $\sigma$ of $[n-1]$.
Set $B=\{ i\in[n-1]: \sigma(i)=i \}$ and $B^{C}=[n-1]\setminus B$.
Consider a term in the expansion of $\det L_{G}^{*}$:
$$
P= (-1)^{\operatorname{sgn}(\sigma)} \prod_{i=1}^{n-1} (L_{G}^{*})_{i\sigma(i)} 
$$
Then we note that:
$$
P=\sum_{\beta}  (-1)^{\operatorname{sgn}(\sigma)+ \lvert B^{C} \rvert } \left( \prod_{i\in B^{C}} A_{i\sigma(i)} \right) \left(\prod_{i\in B} A_{i\beta(i)} \right)
$$
where we sum over all $\beta:B\to[n]$
Suppose that either $\sigma$ has a cycle in $B^{C}$ or $\beta$ has a cycle in $B$.
Take the smallest vertex belonging to one of these cycles.
Now define $\tilde{\sigma}$ and $\tilde{\beta}$ by switching this cycle between $\sigma$ and $\beta$ 
(i.e. if the cycle was in $\sigma$, put it into $\tilde{\beta}$ and vice versa)
Note that $\tilde{\tilde{\sigma}}=\sigma$ and $\tilde{\tilde{\beta}}=\beta$.
Also if this cycle was of odd length, then $\operatorname{sgn}(\sigma)=\operatorname{sgn}(\tilde{\sigma})$, while $2\not\mid\lvert B^{C} \rvert-\lvert \tilde{B}^{C} \rvert$
and if the cycle was of even length, then the opposite holds. 
Either way 
$$
(-1)^{\operatorname{sgn}(\tilde{\sigma})+\lvert \tilde{B}^{C} \rvert } = -(-1)^{\operatorname{sgn}(\sigma)+\lvert B^{C} \rvert }
$$
Thus in the final sum, all of these pairings will cancel eachother out.
The only unpaired terms are when $\sigma=\operatorname{id}$ and $\beta$ has no cycles.
We conclude that 
$$
\det(L_{G}^{*}) = \sum_{\beta} \prod_{i} A_{i\beta(i)}
$$
where we sum over all $\beta:[n-1]\to[n]$ with no cycles.
But these are exactly the spanning trees of $G$ rooted towards $n$.

