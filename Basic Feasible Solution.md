Let $A$ be a $m\times n$ matrix and $b\in \mathbb{R}^{m}$
Let $x$ be a [[Basic Solution]] to $Ax=b$.
We say that $x$ is a basic feasible solution if $x\geq 0$
i.e. $x_{i}>0$ for all $i\in B$ where $B$ is the [[Support]] of $x$
### Lemma
Let $x$ be a BFS to $Ax=b$ with [[Support]] $B$
Let $y$ be a BFS to $Ay=b$ with [[Support]] $B'\subseteq B$
Then $x=y$.
#### Proof
We only need to show that $x$ and $y$ match on the support of $x$.
Let $A'$ be an $m\times \lvert B \rvert$ submatrix of $A$,
taking $i$-th columns of $A$ for each $i\in B$.
By definition of [[Basic Solution]], 
the columns of $A'$ are [[Linearly Independent]].
Thus choose $m$ [[Linearly Independent]] rows of $A'$ 
to build a square $\lvert B \rvert \times \lvert B \rvert$ matrix $A''$
Note that still:
$$
A''x_{B}=A''y_{B}
$$
where $x_{B}$ and $y_{B}$ are taking $i$-th entries of $x$ and $y$ respectively, for each $i\in B$
But now $A''$ is invertible,
so $x_{B}=y_{B}$ and we are done.
## Theorem
Let $S$ be the convex set:
$$
\{ x\in \mathbb{R}^{n} : Ax = b, x\geq 0 \}
$$
A point $x\in S$ is an [[Extreme Point]] of $S$
if and only if 
$x$ is a BFS.
### Proof
#### $\impliedby$
Let $x$ be a BFS with [[Support]] $B_{x}$ and suppose 
$$
x=\lambda y + (1-\lambda)z
$$
where $\lambda \in(0,1)$ and $y,z\in S$ 
i.e. $y,z\geq 0$ and $Ay=Az=b=Ax$
Let $B_{y}$ and $B_{z}$ be [[Support]]s of $y$ and $z$ respectively.
For all $i\not\in B$ we have $x_{i}=0$ and thus $y_{i}=z_{i}=0$
so $B_{y},B_{z}\subseteq B_{x}$
and thus both $y$ and $z$ are [[Basic Solution]]s 
and $y,z\geq 0$ so $y$ and $z$ are BFSs.
By the previous lemma: $x=y=z$ 
and thus $x$ is an [[Extreme Point]] of $S$.
#### $\implies$
Suppose $x\in S$ is an [[Extreme Point]] of $S$.
Let $B$ be the [[Support]] of $x$.
Suppose $Aw=0$ for some vector $w\in \mathbb{R}^{n}$ with support $B'\subseteq B$
Then we can find small enough $\epsilon>0$ such that:
$$
y=x+\epsilon w\geq 0 \quad %quad
\text{and}\quad %quad
z=x-\epsilon w\geq 0
$$
(we can do this as $x_{i}=0\implies w_{i}=0$ by definition)
But now we have $x=0.5y+0.5z$ 
so by definition of [[Extreme Point]] $x=y=z$
and thus $w=0$.
Hence we have proven that the columns of $A_{B}$ are [[Linearly Independent]]
so $x$ is a [[Basic Solution]] and $x\geq 0$ 
so $x$ is a BFS.
