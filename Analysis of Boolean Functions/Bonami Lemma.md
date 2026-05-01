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
\lVert f \rVert _{4}^{4} = \mathop{\Large\mathbb{E}}\limits_{x} (g(x)^{4} + 4\phi_{n}(x)g(x)^{3}h(x)+ 6\phi_{n}(x)^{2}g(x)^{2}h(x)^{2} + 4\phi_{n}(x)^{3}g(x)h(x)^{3} + \phi_{n}^{4} h(x)^{4})
$$
We can drop the second term as $\mathop{\mathbb{E}}\phi_{n}=0$.
In the case $p=q=\frac{1}{2}$ we can also drop the third term and have $\mathop{\mathbb{E}}\phi_{n}^{4}=1$.
In general note:
$$
\begin{gather}
\phi(1)= \sqrt{ \frac{p}{q} } \\
\phi(-1)=\sqrt{ \frac{q}{p} } \\
\lvert\mathop{\mathbb{E}}\phi_{n}^{3}   \rvert = \left\lvert  q \left( \frac{ p }{ q } \right)^{3/2} - p \left( \frac{q}{p} \right)^{3/2}  \right\rvert =\left\lvert  \frac{ p^{2}-q^{2} }{ \sqrt{ qp } }  \right\rvert = \left\lvert  2 \frac{ p-q }{ \sigma }  \right\rvert \leq \frac{2}{\sigma} \\ \\
\mathop{\mathbb{E}}\phi_{n}^{4} = \frac{ p^{3}+q^{3} }{ pq } \leq \frac{4}{\sigma^{2}}
\end{gather}
$$
Now use [[Cauchy-Schwarz Inequality]] and [[Hölder inequality]] to find
$$
\lVert f \rVert _{4}^{4} \leq \lVert g \rVert _{4}^{4} + 6 \lVert \phi_{n} \rVert _{2}^{2} \lVert g \rVert _{2}^{2} \lVert h \rVert _{2}^{2} + \frac{8}{\sigma} 
$$
$$
\mathop{\mathbb{E}}gh^{3}\leq (\mathop{\mathbb{E}}g^{4})^{1/4} (\mathop{\mathbb{E}}h^{4})^{3/4}
$$

