We prove that if $M\models ZFC$ then there is a [[Transitive Model]] $N\subseteq M$
such that 
$$
N\models ZFC+CH
$$
where $CH$ is [[The Continuum Hypothesis]]:
$$
2^{\aleph_{0}}=\aleph_{1}
$$
## Proof
Let $L$ be the [[Constructible Hierarchy]].
Note that 
$$
L\models ZFC
$$
by [[Countable Model of Set Theory]] and [[Consistency of Choice]].
Furthermore $L$ is a [[Transitive Model]] of $ZFC$ and it is minimal.
We will make use of the following lemmas.
### Lemma
If $\alpha\geq \omega$ then $\lvert L_{\alpha} \rvert=\lvert \alpha \rvert$.
#### Proof
By induction on $\alpha$.
Clearly $L_{\omega}$ is countable.
Also $\alpha \subseteq L_{\alpha}$ for all $\alpha \in \mathrm{Or d}$.
Assume that $\lvert L_{\alpha} \rvert=\lvert \alpha \rvert$ and write 
$$
\lvert \alpha+1 \rvert \leq \lvert L_{\alpha+1} \rvert \leq \aleph_{0} \cdot \lvert L_{\alpha}^{<\omega} \rvert = \aleph_{0} \cdot \lvert L_{\alpha} \rvert = \aleph_{0}\cdot \lvert \alpha \rvert  =\lvert \alpha \rvert 
$$
Suppose now $\lambda$ is a limit and for $\alpha<\lambda$, $\lvert L_{\alpha} \rvert=\lvert \alpha \rvert\leq \lvert \lambda \rvert$.
Then write 
$$
\lvert \lambda \rvert  \leq \lvert L_{\lambda} \rvert  =\left\lvert  \bigcup_{\alpha<\lambda} L_{\alpha}  \right\rvert  \leq \lvert \lambda \rvert  \cdot \lvert  \lambda \rvert  =\lvert \lambda \rvert 
$$
### Claim
For every $x\subseteq \mathbb{N}$, $x\in L$, there is some $\alpha<\omega_{1}$ such that $x\in L_{\alpha}$.
#### Proof


