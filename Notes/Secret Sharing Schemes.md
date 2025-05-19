[[Threshold Scheme]]
### Shamir's method
Let $0\leq S\leq N$ be the secret which can be chosen at random 
by the Leader.
The Leader chooses a prime $p>n,N$.
The Leader chooses independent random coefficients
$a_{1},\dots,a_{k-1}$ with $0\leq a_{j}\leq p-1$ where $a_{0}=S$,
and distinct integers $x_{1},\dots,x_{n}$ with $1\leq x_{j}\leq p-1$
Define:
$$
P(r)=a_{0}+\sum_{j=1}^{k-1}a_{j}x_{r}^{j}\pmod{p}
$$
The $r^{th}$ member receives a shadow pair $(x_{r},P(r))$

Now suppose $k$ members are together.
They have the data $(y_{j},Q(j))$ for some $Q$ and can solve:
$$
\begin{pmatrix}
1 & y_{1} & \dots & y_{1}^{k-1} \\
1 & y_{2} & \dots & y_{2}^{k-1} \\
\vdots & \vdots & \ddots & \vdots \\
1 & y_{k} & \dots & y_{k}^{k-1}
\end{pmatrix}
\begin{pmatrix}
z_{0} \\
z_{1} \\
\vdots \\
z_{k}
\end{pmatrix}
=
\begin{pmatrix}
Q(1) \\
Q(2) \\
\vdots  \\
Q(k)
\end{pmatrix}
$$
because the [[Vandermonde matrix]] has nonzero determinant 

