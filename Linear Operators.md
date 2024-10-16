For $X$ and $Y$ [[Normed Spaces]], a linear map $T:X\to Y$ is an operator if it is continuous.
### Proposition
Let $X$, $Y$ be normed, $T:X\to Y$. Then the following are equivalent:
1. $T$ is continuous
2. $T$ is continuous at $0$
3. There is a $k$ such that $\lVert Tx \rVert\leq k\lVert x \rVert$ for all $x \in X$
#### Proof
1=>2 is obvious
2=>3:
$B_{Y}$ is a [[Neighbourhood|nbd]] of 0 in $Y$.
So there is some $\delta>0$ such that $\lVert x \rVert\leq\delta\implies \lVert Tx \rVert\leq 1$.
Now scale up
Thus $\lVert Tx \rVert\leq \frac{1}{\delta}\lVert x \rVert$ for all $x \in X$.
3=>1: $\lVert Tx-Ty \rVert\leq k\lVert x-y \rVert$ so $T$ is uniformly continuous

### Definition
For bounded $T:X\to Y$, the operator norm of $T$ is:
$\lVert T \rVert=\lVert T \rVert_{op}=\sup \{ \lVert Tx \rVert:\lVert x \rVert\leq 1 \}$
This for all $x \in X:\ \lVert Tx \rVert\leq \lVert T \rVert\lVert x \rVert$.

### Definition
Write $L(X,Y)$ for the set of continuous linear maps $X\to Y$ (or $B(X,Y)$). 
Note that $S,T \in L(X,Y)$ then $S+T\in L(X,Y)$.
Indeed $\lVert (S+T)x \rVert\leq \lVert Sx \rVert+\lVert Tx \rVert\leq (\lVert S \rVert+\lVert T \rVert)\lVert x \rVert$ so $S+T$ is bounded. Moreover, $\lVert S+T \rVert\leq \lVert S \rVert+\lVert T \rVert$ so $\lVert  \rVert$ is indeed a norm on $L(X,Y)$.

### Proposition
$X,Y,Z$ normed, $S\in L(X,Y)$ and $T\in L(Y,Z)$. Then $T\circ S\in L(X,Z)$ and $\lVert T\circ S \rVert\leq \lVert T \rVert\lVert S \rVert\lVert x \rVert$.
