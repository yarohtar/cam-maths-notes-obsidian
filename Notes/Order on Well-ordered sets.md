For [[Well-ordering]] sets $X,Y$, write $X\leq Y$ if $X$ is [[Order-isomorphism]] to an [[Initial Segment]] of $Y$ 
### Theorem
Let $X,Y$ be [[Well-ordering]] sets. Then either $X\leq Y$ or $Y\leq X$.

#### Proof
Assume $Y\not\leq X$. Particular $Y\neq \emptyset$
So we can fix $y_{0}\in Y$
Define $f:X\to Y$ by [[Recursive Functions]]:
$$
f(x)=\begin{cases}
min(Y\setminus \{ f(y):y<x \})  & \text{if }Y\setminus \{ f(y):y<x \}\neq \emptyset \\
y_{0} & \text{otherwise}
\end{cases}
$$
Assume the 'otherwise' clause arises. Then there is a least $x$ where it arises. So $f(I_{x})=\{ f(y):y<x \}=Y$
And for all $y<x$
$$
f(y)=min(Y\setminus \{ f(z):z<y \})
$$
As in (previous prop) we show that $f|_{I_{x}}$ is order preserving. So $Y$ is [[Order-isomorphism]] to an [[Initial Segment]] of $X$ 

As in (previous prop) we show $f$ is order-preserving and $im(f)$ is an initial segment of $Y$
Hence $X\leq Y$.

### Proposition
Let $X$, $Y$ be [[Well-ordering]] sets. If $X\leq Y$ and $Y\leq X$ then $X$ is [[Order-isomorphism]] to $Y$ 
#### Proof
Let $f:X\to Y$ and $g:Y\to X$ be [[Order-isomorphism]] to initial segments of $Y$ and $X$ respectively
Then $g\circ f:X\to X$ is an order isomorphism to an [[Initial Segment]] of $X$. By [[Subset Collapse]] and (prop 3?)
$g\circ f=Id_{X}$. Similarly $f\circ g=Id_{Y}$



## Constructing new well ordered sets
[[Extends]]
[[Nested]]
### Proposition
Let $\{ X_{i}:i\in I \}$ be a [[Nested]] set of [[Well-ordering]] sets. Then there is a well ordered set $X$ such that $X_{i}\leq X$ for all $i\in I$