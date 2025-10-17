Let $A$ be a $m\times n$ matrix and $b\in \mathbb{R}^{m}$
Let $x\in \mathbb{R}^{n}$ such that $Ax=b$
The [[Support]] of $x$ is:
$$
B=\{ i\in[n] : x_{i}\neq 0 \}
$$
we say $x$ is a basic solution if the columns of $A_{B}$ are [[Linearly Independent]]
where $A_{B}$ is a $m\times \lvert B \rvert$ submatrix of $A$, 
built by taking $i$-th column of $A$ iff $i\in B$

Note that by definition we have $\lvert B \rvert\leq m\leq n$.
