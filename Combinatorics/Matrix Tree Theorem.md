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
