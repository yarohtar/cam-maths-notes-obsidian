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

