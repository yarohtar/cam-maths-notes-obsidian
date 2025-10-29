Let $X$ and $Y$ be [[Random Variable]]s 
taking values in $\Sigma_{1}$ and $\Sigma_{2}$ respectively.
The joint entropy of $X$ and $Y$ is 
$$
H(X,Y) = \mathbb{E}(-\log I(X,Y))
$$
where $I$ is the [[Information Content]].
Expanding:
$$
H(X,Y)=-\sum_{x\in \Sigma_{1}}\sum_{y\in \Sigma_{2}}P(x,y)\log P(x,y)
$$
where $P$ is their joint distribution.
### Lemma
$$
H(X,Y)\leq H(X)+H(Y)
$$
with equality if and only if $X$ and $Y$ are [[Independent]] 
#### Proof
$\Sigma_{1}=\{ x_{1},\dots,x_{n} \}$ and $\Sigma_{2}=\{ y_{1},\dots,y_{n} \}$
$p_{ij}=P(X=x_{i},Y=y_{j})$, $p_{i}=P(X=x_{i})$, $q_{j}=P(Y=y_{j})$
Apply Gibbs' inequality with distributions $p_{ij}$ and $p_{i}q_{j}$
$$
\begin{align}
-\sum p_{ij}\log(p_{ij}) & \leq-\sum p_{ij}\log(p_{i}q_{j}) \\
 & =-\sum_{i}\left( \sum_{j}p_{ij} \right)\log p_{i}-\sum_{j}\left( \sum_{i}p_{ij} \right)\log q_{j} \\
 & =-\sum_{i}p_{i}\log p_{i}-\sum q_{j}\log q_{j}
\end{align}
$$
i.e. 
$$
H(X,Y)\leq H(X)+H(Y)
$$
Equality $\iff p_{ij}=p_{i}q_{j}$ for all $i,j$ $\iff$ $X$ and $Y$ are independent.
