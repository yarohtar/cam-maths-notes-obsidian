Let $m_{1}\dots m_{k}$ be positive integers which are pairwise coprime. Let $M=m_{1}\dots m_{k}$.
### Theorem
 Let $a_{1}\dots a_{k}\in \mathbb{Z}$. Then there exists a solution $x \in \mathbb{Z}$ to the system of simultaneous congruences $x\equiv a_{i}\pmod{m_{i}}$. Moreover this solution is unique modulo $M$.
#### Proof

### Theorem
The map:
$$
\begin{align}
\theta: \mathbb{Z}/M\mathbb{Z}&\to(\mathbb{Z}/m_{1}\mathbb{Z})\times\dots \times(\mathbb{Z}/m_{k}\mathbb{Z}) \\
(a+M\mathbb{Z})&\to(a+m_{1}\mathbb{Z},\dots,a+m_{k}\mathbb{Z})
\end{align}
$$
is a [[Rings|ring]] isomorphism.
#### Proof
We just need to check that its bijective, but this is exactly the previous theorem.
### Corollary
There is a group isomorphism
$$
(\mathbb{Z}/M\mathbb{Z})^\times \cong \left(\mathbb{Z}/m_{1}\mathbb{Z} \right)^\times\dots \times(\mathbb{Z}/m_{k}\mathbb{Z})^\times
$$
#### Proof
Just look at components, its fine.