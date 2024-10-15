Let $\Pi_{n}$ be the space of all bi-infinite complex $n$-periodic sequences $x=\{ x_{l} \}_{l\in \mathbb{Z}}$ (such that $x_{l+n}=x_{l}$). Set $\omega_{n}=\exp \frac{2\pi i}{n}$ the primitive root of unity of degree $n$. The discrete Fourier transform (DFT) of $x$ is:

$$
FF_{n}:\Pi_{n}\to \Pi_{n}
$$
such that
$$
y=FF_{n}x
$$
where
$$
y_{j}=\frac{1}{n}\sum_{l=0}^{n-1} \omega_{n}^{-jl}x_{l}
$$
where $j=0\dots n-1$