Every non constant polynomial over $\mathbb{C}$ has a root in $\mathbb{C}$.

#### Proof
By contradiction.
Let $p(z)=z^n+a_{1}z^{n-1}+\dots+a_{n}$ with no root, $n\geq 1$ (wlog monic)

Take $R\gg 0$ st $R>max\left( \sum \lvert a_{i} \rvert, 1 \right)$
On $\lvert z \rvert=R$, there can be no roots.
Let $p_{t}(z)=z^n+t(a_{1}z^{n-1}+\dots+a_{n})$ for $t\in[0,1]$.
Then $p_{t}$ also has no roots in $\lvert z \rvert=R$.
Define:
$$
\begin{align}

F:I\times I&\to S^1 \\
(s,t) & \to \frac{p_{t}(\mathrm{Re}^{2\pi is}) / p_{t}(R)}{\lvert p_{t}(\mathrm{Re}^{2\pi is}) / p_{t(R)} \rvert }
\end{align}
$$
Well defined because $p_{t}$ is non zero ..
$F(0,t)=F(1,t)=1$
$F$ is a homotop