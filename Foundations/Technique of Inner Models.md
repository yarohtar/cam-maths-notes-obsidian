The [[Constructible Hierarchy]] $L$ is the [[Constructible Model of Set Theory]]:
$$
L\models ZF
$$
Also, by [[Consistency of Choice]]:
$$
L\models ZFC
$$
Furthermore $L$ is countable [[Transitive Model|Transitive]].
We now prove stuff inside $L$.
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
### Lemma
For every $x\subseteq \mathbb{N}$, $x\in L$, there is some $\alpha<\omega_{1}$ such that $x\in L_{\alpha}$.
#### Proof
We work in $L$.
Let $B_{x} = \mathbb{N}\cup \{ x \}$ and note that this is a [[Foundations/Set Theory/Transitive|Transitive]] set.
Find $\nu$ large enough by [[Lévy Reflection Theorem]] 
such that $x\in L_{\nu}$ and $\sigma$ is absolute between $L_{\nu}$ and $L$ 
where $\sigma$ is from [[Gödel's Condensation Lemma]].
Because $L\models \sigma$, we get $L_{\nu}\models \sigma$.
Now using [[The Downward Löwenheim-Skolem Theorem]]
find $M$ such that $B_{x}\subseteq M\subseteq L_{\nu}$ with $\sigma$ [[Absolute]] between $M$ and $L_{\nu}$.
So $M\models \sigma$ and $M$ is countable.
Form the [[Transitive Model|Transitive]] $N\cong M$ by [[Mostowski's Collapsing Theorem]].
Then by [[Gödel's Condensation Lemma]], there is some $\alpha$ such that $N=L_{\alpha}$
Since $N$ is countable, it has to be $\alpha<\omega_{1}$.
### Theorem
[[The Continuum Hypothesis]] holds in $L$: 
$$
L\models ZFC+CH
$$
#### Proof
By the previous lemma, all subsets of $\mathbb{N}$ are contained in $L_{\omega_{1}}$.
Furthermore, $\lvert L_{\omega_{1}} \rvert=\lvert \omega_{1} \rvert$.
Thus the powerset of $\mathbb{N}$ is of cardinality at most $\lvert \omega_{1} \rvert$.
