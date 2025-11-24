Let $\mathcal{D}(X)$ be [[Constructible Sets]] from a set $X$.
Define now 
$$
\begin{gather}
L_{0} = \varnothing  \\
L_{\alpha+1} = \mathcal{D}(L_{\alpha}) \\
L_{\lambda} = \bigcup_{\alpha<\lambda} L_{\alpha} \\
L=\bigcup_{\alpha \in \mathrm{Or d}} L_{\alpha}
\end{gather}
$$
Note that $L$ is a [[Hierarchy]].
[[Constructible Rank]]
## Lemma
For $\alpha\leq \omega$ we have $L_{\alpha}=V_{\alpha}$ where $V$ is the [[Von Neumann Hierarchy]].
For $\alpha>\omega$ then $L_{\alpha}\neq V_{\alpha}$.
### Proof
First bit by $\omega$-induction.
Then $L_{\omega}=\bigcup_{\alpha<\omega}L_{\alpha}=\bigcup_{\alpha<\omega}V_{\alpha}=V_{\omega}$.
However, $L_{\omega+1}$ is countable and $V_{\omega+1}$ is not.
## Lemma
$L$ is [[Absolute]] for [[Transitive Model]]s of a [[Sufficiently Strong]] $T$
i.e. there is a formula $\Gamma$ such that $\Gamma(\alpha,x)$ if and only if $x\in L_{\alpha}$.
This $\Gamma$ is [[Absolute]] for $L$.
### Proof
The definition of $L$ is recursive.
## Corollary
Let $T$ be [[Sufficiently Strong]] for [[Absolute]]ness of $\Gamma$ (above).
Let $N$ be a [[Transitive Model]] of $T$.
Then 
$$
\bigcup_{\alpha \in N\cap \mathrm{Or d}} L_{\alpha} \subseteq N
$$
### Proof
Let $\alpha \in N\cap \mathrm{Or d}$.
Note that $\alpha \to L_{\alpha}$ is an [[Absolute Operation]] and thus $L_{\alpha}\in N$.
As $N$ is [[Foundations/Set Theory/Transitive|Transitive]], we know that $L_{\alpha}\subseteq N$.
