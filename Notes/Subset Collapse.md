Let $Y$ be a [[Well-ordering]] set and $X\subseteq Y$
Then there is a unique [[Initial Segment]] of $Y$ which is [[Order-isomorphism]] to $X$ 

#### Proof
##### Uniqueness 
Assume $f$ is an order isomorphism from $X$ to an initial segment of $Y$ 
By lemma ? 
$$
f(x)=min(Y\setminus \{ f(y):y<x \})
$$
for all $x\in X$
By [[Proof by Induction]], $f$ is uniquely determined 
##### Existence
WLOG $Y\neq \emptyset$
Fix $y_{0}\in Y$
Define $f:X\to Y$ by recursion
$$
f(x)=\begin{cases}
min(Y\setminus \{ f(y):y<x \}) & \text{if }Y\setminus \{ f(y):y<x \}\neq \emptyset \\
y_{0} & \text{otherwise}
\end{cases}
$$
We first prove that the 'otherwise' clause does not arise
We do this by proving that $f(x)\leq x$ for all $x\in X$
(by induction)
Fix $x\in X$ and assume $f(y)\leq y$ for all $y<x$
Then $x\in Y\setminus \{ f(y):y<x \}$ and hence $f(x)\leq x$

Fix $y<x$