Let $T$ be a [[Theory]] which encodes natural numbers (e.g. $ZFC$ or $PA$)
We can encode formulas and proofs in $T$ with these numbers
so that every proof and/or formula is just a number in $\omega$
Define 
$$
\mathrm{Cons}(T) = (\forall n\in \omega)\, n \text{ is not the proof of } T\vdash \bot
$$
## Theorem 1
There is some formula $G$ such that if $\mathrm{Cons}(T)$
then $T\not\vdash G$ and $T\not\vdash \neg G$.
### Proof
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
Note that 
$$
(\forall n\in \omega)\, q(n,y)
$$
means that $T\not\vdash F(y)$ (if $y$ is an encoding of $F$ with one [[Free Variable]])
and it is itself a formula in one [[Free Variable]].
Let $z$ be the encoding of 
$$
F=(\forall n\in \omega)\, q(n,y)
$$
Then 
$$
q(n,z)
$$
says that $n$ is not a proof of $F(z)$ i.e. $n$ is not a proof of
$$
(\forall n\in \omega)\, q(n,z)
$$
Let $G=(\forall n\in \omega)\,q(n,z)$


$$
(\forall n\in \omega)\, q(n,z)
$$
says that $T\not\vdash(\forall n\in \omega)\,q(n,z)$, in particular
$$
T\vdash(\forall n\in \omega)\,q(n,z) \implies (\forall n\in \omega) \neg R(n, z)
$$
We claim that $F=(\forall n\in \omega)\,q(n,z)$ is what we are looking for.
Suppose $T\vdash F$.
Then 
$$
T\vdash(\forall n\in \omega)\neg R(n,z)
$$
But we can find $n$ such that $n$ encodes the proof of $F$ i.e. $R(n,z)$ which is a contradiction.
Now suppose $T\vdash \neg F$.
But then there is some $n$ such that $\neg q(n,z)$ 
i.e. there is some $n$ such that $n$ is a proof of $(\forall n\in \omega)q(n,z)$ 
But then $T\vdash F$ which is again a contradiction.
We conclude that if $\mathrm{Cons}(T)$ then
$$
T\not\vdash F\text{ and }T\not\vdash \neg F
$$
## Theorem 2
$$
T\not\vdash \mathrm{Cons}(T)
$$
### Proof
Suppose
$$
T\vdash \mathrm{Cons}(T)
$$
Then $T$ proves that 
$$
T\not\vdash F \text{ and } T\not\vdash \neg F
$$
from the first theorem.
In particular
$$
T\vdash(\forall n\in \omega)\,q(n,z)
$$
but then $T\vdash F$ which is a contradiction.


