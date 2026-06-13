Let $B$ be a [[Boolean Algebra]] and $\mathcal{U}$ an [[Ultrafilter]] on $B$.
In particular:
$$
\begin{gather}
a\in \mathcal{U}\land a\leq b\implies b\in \mathcal{U} \\
a\in \mathcal{U} \land b\in \mathcal{U} \iff a\land b\in \mathcal{U} \\
a \in \mathcal{U} \iff \neg a\not\in \mathcal{U}
\end{gather}
$$
(the last property is easy but not trivial)
### Lemma
An [[Ultrafilter]] on $B$ is a homomorphism to $\{ 0,1 \}$.
#### Proof
Let $\mathcal{U}$ be an [[Ultrafilter]] on a [[Boolean Algebra]] $B$.
We prove that the characteristic function $u$ of $\mathcal{U}$ is a homomorphism:
$$
u(a\land b)=1 \iff a\land b\in \mathcal{U} \iff a\in \mathcal{U}\land b\in \mathcal{U} \iff u(a)=1 \land u(b)=1
$$
[[Stone Space]]



 