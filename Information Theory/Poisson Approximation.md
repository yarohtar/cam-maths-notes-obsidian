Suppose $X_{1},X_{2},\dots,X_{n}$ are binary [[Random Variable]]
with each $X_{i}\sim \mathrm{Bern}(p_{i})$ and let $\lambda=\sum_{i}p_{i}$.
Let
$$
S_{n}=\sum_{i} X_{i}
$$
and let $P_{S_{n}}$ be its distribution. Then:
$$
D_{e}(P_{S_{n}}||\Pi_{\lambda}) \leq \sum_{i=1}^{n} p_{i}^{2} + \left( \sum_{i=1}^{n} H_{e}(X_{i}) - H_{e}(X_{1},\dots,X_{n}) \right)
$$
where $D_{e}$ is [[Relative Entropy]] and $H$ is [[Mathematical Entropy]].
#### Proof
Let $Z_{1},Z_{2},\dots,Z_{n}$ be [[Independent]] with each other and 
$$
Z_{i} \sim \mathrm{Po}(p_{i})
$$
and let
$$
T_{n} = \sum_{i=1}^{n} Z_{i} \sim \mathrm{Po}(\lambda)
$$
Now use [[Data Processing Property of the Relative Entropy]] to find:
$$
\begin{align}
D_{e}(P_{S_{n}}||\Pi_{\lambda})  & = D_{e}(P_{S_{n}}|| P_{T_{n}}) \\
 & \leq D_{e}(P_{X_{i}^{n}}|| P_{Z_{1}^{n}})  \\
 & = \sum_{x_{1}^{n}} P_{x_{1}^{n}}(x_{1}^{n}) \log_{e} \left(  \frac{ P_{x_{1}^{n}}(x_{1}^{n}) }{ \prod_{i=1}^{n} P_{Z_{i}}(x_{i}) } \frac{ \prod_{i=1}^{n} P_{x_{i}^{n}} }{ \prod_{i=1}^{n} P_{X_{i}}(x_{i}) } \right) \\
 & = \sum_{x_{1}^{n}} P_{x_{1}^{n}} \log_{e} \left( \prod_{i} \frac{ P_{X_{i}} }{ P_{Z_{i}} }  \right) + \sum P_{x_{1}^{n}}\log_{e} P_{x_{1}^{n}} - \sum P_{x_{1}^{n}} \log_{e} \left( \prod_{i} P_{x_{i}} \right)  \\
 & = \sum_{i} D_{e}(P_{x_{i}}||P_{x_{i}}) + \left( \sum_{i} H_{e}(x_{i}) - H_{e}(x_{1}^{n}) \right)
\end{align}
$$
where
$$
\begin{align}
D_{e}(P_{X_{i}}||P_{Z_{i}}) & = D_{e}(\mathrm{Bern}(p_{i})||\mathrm{Po}(p_{i}))  \\
 & =p_{i}\log_{e} \frac{ p_{i} }{ p_{i}e^{p_{i}} }  + \dots \\
 & \leq \dots p_{i}^{2}
\end{align}
$$
### Corollary
If $X_{i}$ as above are IID with $X_{i}\sim \mathrm{Bern}\left( \frac{\lambda}{n} \right)$ then:
$$
\frac{1}{2} \lVert P_{S_{n}} - \Pi_{\lambda} \rVert ^{2}_{TV} \leq D_{e}(P_{S_{n}}||\Pi_{\lambda}) \leq \frac{ \lambda^{2} }{ n }
$$
for all $n$, where $\lVert \cdot \rVert_{TV}$ is [[Total Variation Distance]].
#### Proof
Apply [[Pinsker's Inequality]].

### Corollary
$$
H(\mathrm{Po}(\lambda)) = \sup \{ H(P) :  \}
$$

