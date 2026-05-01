Let $f:\{ -1,1 \}^{n}\to \mathbb{R}$ be a function on the $p$-[[Biased Cube]]
Then define
$$
D_{i}f(x) = \frac{\sigma}{2} (f(x_{i\to 1}) - f(x_{i\to-1}))
$$

### Lemma
$$
D_{i}\phi_{A}(x) = \begin{cases}
\phi_{A\setminus \{ i \}}  &  \text{if $i\in A$}\\
0 & \text{otherwise}
\end{cases}
$$
### Lemma
If $\hat{f}$ is the [[Discrete Fourier Transform on the Biased Cube]], then:
$$
D_{i}f=\sum_{A\ni i} \hat{f}(A)\phi_{A\setminus \{ i \}}
$$