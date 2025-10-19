Let $A$ be a $m\times n$ matrix and $b\in \mathbb{R}^{m}$
Let $x\in \mathbb{R}^{n}$ such that $Ax=b$
The [[Support]] of $x$ is:
$$
S=\{ i\in[n] : x_{i}\neq 0 \}
$$
we say $x$ is a basic solution if the columns of $A_{S}$ are [[Linearly Independent]]
where $A_{S}$ is a $m\times \lvert S \rvert$ submatrix of $A$, 
built by taking $i$-th column of $A$ iff $i\in S$

Note that by definition we have $\lvert S \rvert\leq m\leq n$.
## Lemma
Let $A\in \mathbb{R}^{m\times n}$ be a matrix of rank $m$ and $b\in \mathbb{R}^{m}$
Let $B\subseteq[n]$ be a set of size $\lvert B \rvert=m$ such that $A_{B}$ is invertible.
Then there exists a unique [[Basic Solution]] to $Ax=b$ with [[Basis]] $B$.
Conversely, let $x$ be a [[Basic Solution]] to $Ax=b$.
Then there exists a $B\subseteq[n]$ such that $x$ has [[Basis]] $B$.
### Proof
Using lemmas in [[Basis]].
