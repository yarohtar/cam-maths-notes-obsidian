The [[Constructible Hierarchy]] $L$ is the [[Constructible Model of Set Theory]]:
$$
L\models ZF
$$
Also, by [[Consistency of Choice]]:
$$
L\models ZFC
$$
Furthermore $L$ is [[Transitive Model|Transitive]] and [[Axiom of Constructability]] is [[Satisfied]]:
$$
L\models V=L
$$
We now prove stuff inside of $L$.
### General Idea
Suppose we can prove that 
$$
L\models \varphi
$$
Then we claim that 
$$
\mathrm{Cons}(ZF) \implies \mathrm{Cons}(ZF + \varphi)
$$
#### Proof
Let $V$ be the set theoretic universe, i.e. 
$$
V \models ZF
$$
Assume $\mathrm{Cons}(ZF)$.
Let $T\subseteq ZF$ be finite and [[Sufficiently Strong]] to prove
1. [[Absolute]]ness of $L$
2. [[Absolute]]ness of formula and proof encodings and such

Furthermore, find a finite $T^{*}\supseteq T$, $T^{*}\subseteq ZF$
such that if $M\models T^{*}$, then $L^{M}\models T$.
Find a [[Countable Transitive Model]] $M$ of $T^{*}$.
Let $L^{M}$ be the [[Constructible Hierarchy]] in $M$.
Now inside of $M$, we can run the proof of 
$$
L^{M}\models T + \varphi
$$
But $L^{M}$ is just a fragment of the real $L$ and in particular $L^{M}$ is a set.
As all the proofs and formulas are [[Absolute]], 
so the real universe $V$ also proves that 
$$
L^{M} \models T + \varphi
$$
Thus $V$ can find a set model of any finite fragment of $ZF+\varphi$.
We conclude that 
$$
V\models \mathrm{Cons}(ZF+\varphi)
$$

Then $V$ thinks there is a [[Model]] $M$ of $ZF$, where $M$ is a set $M\in V$.
This is because we can run the argument from [[Model Existence Lemma]] in $V$.
(note that this uses [[Axiom of Choice]], 
but we are fine because $V$ can [[Well-Ordered|Well-Order]] formulas)
Assume also $\neg \mathrm{Cons}(ZF+\varphi)$, so that
$$
ZF\vdash \neg \mathrm{Cons}(ZF+\varphi)
$$ 
Now as $M$ is a [[Model]] of $ZF$ it has to be:
$$
M\models \neg \mathrm{Cons}(ZF+\varphi)
$$
Let $L$ be the [[Constructible Hierarchy]] in $M$.
Note that we can prove (from $M$) that 
$$
L\models ZF + \varphi
$$

### Lemma (main idea)
For every $x\subseteq \mathbb{N}$, $x\in L$, there is some $\alpha<\omega_{1}$ such that $x\in L_{\alpha}$.
#### Proof
We work in $L$, which is a [[Model]] of $ZFC$.
Let $B_{x} = \mathbb{N}\cup \{ x \}$ and note that this is a [[Foundations/Set Theory/Transitive|Transitive]] set.
Find $\nu$ large enough by [[Lévy Reflection Theorem]] 
such that $x\in L_{\nu}$ and $\sigma$ is absolute between $L_{\nu}$ and $L$ 
where $\sigma$ is from [[Gödel's Condensation Lemma]].
Because $L\models \sigma$, we get $L_{\nu}\models \sigma$.
Now using [[The Downward Löwenheim-Skolem Theorem]]
find countable $M$ such that $B_{x}\subseteq M\subseteq L_{\nu}$ with $\sigma$ [[Absolute]] between $M$ and $L_{\nu}$.
So $M\models \sigma$ and $M$ is countable.
Form the [[Transitive Model|Transitive]] $N\cong M$ by [[Mostowski's Collapsing Theorem]].
Then by [[Gödel's Condensation Lemma]], there is some $\alpha$ such that $N=L_{\alpha}$
Since $N$ is countable, so is $L_{\alpha}$.
But $\lvert L_{\alpha} \rvert=\lvert \alpha \rvert$, so it has to be $\alpha<\omega_{1}$.
### Theorem
[[The Continuum Hypothesis]] holds in $L$: 
$$
L\models ZFC+CH
$$
#### Proof
By the previous lemma, all subsets of $\mathbb{N}$ are contained in $L_{\omega_{1}}$.
Furthermore, $\lvert L_{\omega_{1}} \rvert=\lvert \omega_{1} \rvert$.
Thus the powerset of $\mathbb{N}$ is of cardinality at most $\lvert \omega_{1} \rvert$.
