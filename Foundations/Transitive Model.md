---
aliases:
  - Transitive
---
Suppose $(M,E)$ and $(N,E)$ are $\mathcal{L}$-[[Structure]]s,
where $\mathcal{L}$ is the [[Language]] of set theory i.e. $\mathcal{L}=\{ \in \}$
and $M\subseteq N$
We say that $M$ is transitive in $N$ if 
for any $x,y\in N$ such that
- $y\in M$
- $xEy$ (in $N$)
implies that $x\in M$

### Lemma
If $N$ is the set theoretic universe (in [[Zermelo-Fraenkel Set Theory]])
then $M$ is transitive in $N$ 
if and only if
$M$ is a [[Foundations/Set Theory/Transitive|Transitive]] set.
### Lemma
Let $N$ be the set theoretic universe.
If $M$ is transitive then $(M,\in)\models$ [[Axiom of Extensionality]] + [[Axiom of Foundation]]
#### Proof
##### Extensionality
$$
\forall x\,\forall y\,(\forall w\,(w\in x \iff w\in y)\implies x=y)
$$
Let $x,y\in M$ such that $x\neq y$
By [[Axiom of Extensionality]] (in $N$) there is (WLOG) some $z\in x\setminus y$ 
Now by [[Foundations/Set Theory/Transitive|Transitivity]] of $M$ we know $z\in x$ and $x\in M$ so $z\in M$
Thus
$$
\begin{gather}
M\models z\in x \land z\not\in y \\
M\models \neg(\forall w)(w\in x \iff w\in y)
\end{gather}
$$
##### Foundation
$$
\forall x\,(x\neq \varnothing \implies \exists m\,)
$$

