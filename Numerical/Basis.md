Let $x\in \mathbb{R}^{n}$ be a [[Basic Solution]] to $Ax=b$ with [[Support]] $S$
where $A\in \mathbb{R}^{m\times n}$ and $b\in \mathbb{R}^{m}$
The basis of $x$ is a set $B\subseteq[n]$ such that:
- $S\subseteq B$
- $\lvert B \rvert=m$
- and $A_{B}$ is invertible
where $A_{B}$ is the $m\times m$ submatrix of $A$ 
formed by taking $i$-th column of $A$ when $i\in B$
## Lemma
Suppose $x$ and $y$ are [[Basic Solution]]s to $Ax=b$
with the same [[Basis]].
Then $x=y$.
### Proof
Suppose $x$ and $y$ have basis $B$ and [[Support]]s $S_{x}$ and $S_{y}$ respectively.
Then by definition, $S_{x},S_{y}\subseteq B$.
Now $x_{i}=y_{i}=0$ for $i\not\in B$
and $x_{B}=y_{B}=A_{B}^{-1}b$
where $A_{B}$ is invertible by definition.
## Lemma
Suppose $A\in \mathbb{R}^{m\times n}$ has rank $m$ (i.e. all its rows are [[Linearly Independent]])
Then for any [[Basic Solution]] $x$, there exists a basis.
### Proof
Suppose [[Basic Solution]] $x$ has [[Support]] $S$. 
Columns of $A_{S}$ are [[Linearly Independent]] by definition, so $\lvert S \rvert\leq m$
Let $V_{A}$ be the space spanned by the columns of $A$.
It has dimension $m$ (due to rank of $A$ being $m$)
If the columns of $A_{S}$ span $V_{A}$, then $\lvert S \rvert\geq m$ and thus $\lvert S \rvert=m$
so $S$ is a [[Basis]] of $x$

If the columns of $A_{S}$ do not span $V_{A}$
then pick a column of $A$ not in $\operatorname{span}A_{S}$ with index $i$
and form the set $S\cup \{ i \}$
Repeat this process until we arrive at a [[Basis]].

