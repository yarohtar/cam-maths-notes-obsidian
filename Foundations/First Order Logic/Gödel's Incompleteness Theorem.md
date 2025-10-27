Let $T$ be a [[Theory]] which encodes natural numbers (e.g. $ZFC$ or $PA$)
We can encode formulas and proofs in $T$ with these numbers.
Define 
$$
\mathrm{Cons}(T) = (\forall n\in \omega)\, n \text{ is not the proof of } T\vdash \bot
$$
Then 
$$
T\not\vdash \mathrm{Cons}(T)
$$
### Proof
Suppose
$$
T\vdash \mathrm{Cons}(T)
$$
Define a relation on $\omega$ given by $R(x,y)$ if and only if $x$ is a proof of $y$
(where $x$ is decoded as a proof, and $y$ is decoded as a formula)
For any $n\in \omega$ and $F$ a formula with one [[Free Variable]], 
let $y$ be the encoding of $F$ and let
$$
q(n,y)=\begin{cases}
1  & \text{if }\neg R(n,F(y)) \\
0 & \text{ otherwise}
\end{cases}
$$
i.e. $q(n,y)$ if and only if $n$ is not the proof of $F(y)$ 
Thus let 
$$
F = x\text{ is not the proof of }T\vdash\bot
$$
a formula with one free variable $x$.
Let $y$ be the encoding of $F$.
Examine $q(y,y)$.
If $q(y,y)=1$ then $\neg R(y,F(y))$ i.e. $y$ is not a proof of $F(y)$ 
If $q(y,y)=0$ then $R(y,F(y))$ i.e. $y$ is a proof of
$$
y \text{ is not the proof of }T\vdash \bot
$$

 