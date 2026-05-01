Let $f:\{ -1,1 \}^{n}\to \mathbb{R}$ be a function on the $p$-[[Biased Cube]] 
with [[Degree of a Boolean Function]] at most $k$.
Then
$$
\lVert f \rVert _{4} \leq C^{k/2}\lVert f \rVert _{2}
$$
#### Proof
By induction on $n$.
Let $g=E_{n}f$ and $h=D_{n}f$ as in [[Discrete Derivative]].
By orthogonality:
$$
\lVert f \rVert _{2}^{2} = \lVert g \rVert _{2}^{2} + \lVert \phi_{n}h \rVert _{2}^{2} = \lVert g \rVert _{2}^{2} + \lVert h \rVert _{2}^{2}
$$
Note also that $D_{n}f$ has degree at most $k-1$ as
$$
D_{n}f = \sum_{A\ni n} \hat{f}(A)\phi_{A\setminus \{ i \}}
$$
So 
$$
\lVert f \rVert _{4}^{4} = \mathop{\Large\mathbb{E}}\limits_{x} (g(x)^{4} + 4\phi_{n}(x)g(x)^{3}h(x)+ 6\phi_{n}(x)^{2}g(x)^{2}h(x)^{2} + 4\phi_{n}(x)^{3}g(x)h(x)^{3} + h(x)^{4})
$$
We can drop the second term as $\mathop{\mathbb{E}}\phi_{n}=0$.

