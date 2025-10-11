Let $X$ be a topological space. We say it is disconnected if we can find open $U$ and $V$ s.t. $U\cap V=\emptyset$, $U\cup V=X$ and they are nonempty.

We say $X$ is connected if it is not disconnected.

The image of a [[Continuity in topological spaces|continuous]] function on a connected set is connected.

The following are equivalent:
1. $X$ is connected
2. If $f:X\to\mathbb R$ then $f(X)$ is an interval
3. Every cts function $f:X\to D$ where $D$ is discrete and $|D|\geq 2$ is constant

A subspace $Y$ of $X$ is disconnected iff there are open sets $U,V$ in $X$ s.t. $U\cap Y\neq\emptyset$, $V\cap Y\neq\emptyset$, $Y\subseteq U\cup V$ and $U\cap V\cap Y=\emptyset$.

If $X$ is connected with equivalence relation $R$ then $X/R$ is connected.
([[Quotient space|quotient map]] is cts)

## Path-connected
A space $X$ is path-connected if for any $x,y\in X$, there is a cts function $\gamma:[0,1]\to X$ s.t. $\gamma(0)=x$ and $\gamma(1)=y$.
Any path-connected space is connected. (Converse is not true).

![[Gluing lemma]]

### Theorem
Let $U\subseteq\mathbb R^n$ be open. Then $U$ is connected iff $U$ is path-connected.
#### Proof sketch
WLOG $U\neq\emptyset$. Find $x_0\in U$. Let $V$ be path-connected component of $x_0$. We show $V$ and $U\setminus V$ are open in $U$. Then they would disconnect it, unless $V=U$.