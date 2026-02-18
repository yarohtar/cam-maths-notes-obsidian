For any positive integers $r, k$, there exists a smallest integer $R(r, k)$ such that if the edges of the complete graph $K_n$ on $n \geq R(r, k)$ vertices are colored with $k$ colors, then there is a monochromatic clique of size $r$.

## Proof (by induction on $r$)

The case $r=1$ is trivial. Assume for $r-1$.

Let $$n = R(r-1, k) + R(r, k-1) - 1$$.

Consider a $k$-coloring of $K_n$.

Fix a vertex $v$. The edges from $v$ to other vertices are colored with $k$ colors, so by pigeonhole, some color $c$ is used at least $\lceil (n-1)/k \rceil$ times.

Let $S$ be the set of vertices connected to $v$ by color $c$, with $|S| \geq R(r-1, k)$.

If $S$ has a monochromatic clique of size $r-1$ in color $c$, then adding $v$ gives a monochromatic $K_r$ in color $c$.

Otherwise, the subgraph induced by $S$ has no monochromatic $K_{r-1}$ in color $c$, but since it's colored with $k-1$ colors (excluding $c$), by induction, there is a monochromatic $K_r$ in one of the other colors.

## Corollary

Ramsey numbers exist for any finite parameters.

#ai-generated