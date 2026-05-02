Let $X_{1},\dots ,X_{n}$ and $Y_{1},\dots,Y_{n}$ be sequences of [[Independent]] [[Random Variable]]s.
Suppose that $\mathop{\mathbb{E}}X_{i}=\mathop{\mathbb{E}}Y_{i}$ and $\mathop{\mathbb{E}}X_{i}^{2}=\mathop{\mathbb{E}}Y_{i}^{2}$ for all $i$.
Let $\psi:\mathbb{R}\to \mathbb{R}$ have a third derivative and:
$$
\lVert \psi''' \rVert _{\infty} \leq C
$$
Then
$$
\lvert \mathop{\mathbb{E}}\psi(X_{1}+\dots+X_{n})-\mathop{\mathbb{E}}\psi(Y_{1}+\dots +Y_{n}) \rvert  \leq C \left( \sum_{i=1}^{n} (\lVert X_{i} \rVert _{3}^{3} + \lVert Y_{i} \rVert _{3}^{3}) \right)
$$
#### Proof
Write $U_{i}=X_{1}+\dots+X_{i-1}+Y_{i+1}+\dots+Y_{n}$.
By triangle inequality we have 
$$
\lvert \mathop{\mathbb{E}}\psi(U_{n}+X_{n}) - \mathop{\mathbb{E}}\psi(U_{1}+Y_{1}) \rvert \leq \sum_{i=1}^{n} \lvert \mathop{\mathbb{E}}\psi(U_{i}+X_{i}) -\mathop{\mathbb{E}}\psi(U_{i}+Y_{i}) \rvert 
$$
By [[Taylor's theorem]]:
$$
\psi(U_{i}+X_{i}) =\psi(U_{i}) + X_{i} \psi'(U_{i}) + \frac{ X_{i}^{2} }{ 2 } \psi''(U_{i}) + \frac{ X_{i}^{3} }{ 6 } \psi'''(V_{i}) 
$$
where $V_{i}$ is between $U_{i}$ and $U_{i}+X_{i}$ and similar for $\psi(U_{i}+Y_{i})$
Taking expectations and substracting, the first $3$ terms cancel so we are left with:
$$
\mathop{\mathbb{E}}\psi(U_{i}+X_{i}) - \mathop{\mathbb{E}}\psi(U_{i}+Y_{i}) = \frac{1}{6}(\mathop{\mathbb{E}}X_{i}^{3}\psi'''(V_{i}) - \mathop{\mathbb{E}} Y_{i}^{3}\psi'''(W_{i}))
$$
which has size at most 
$$
\frac{C}{6}(\mathop{\mathbb{E}})
$$
$$
\lvert \mathop{\mathbb{E}}\psi(U_{n}+X_{n}) - \mathop{\mathbb{E}}\psi(U_{1}Y_{1}) \rvert \leq \sum_{i=1}^{n} \mathop{\mathbb{E}}
$$