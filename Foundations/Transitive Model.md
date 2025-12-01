---
aliases:
  - Transitive
---
Suppose $(M,E)$ and $(N,E)$ are $\mathcal{L}$-[[Foundations/First Order Logic/Structure|Structure]]s,
where $\mathcal{L}$ is the [[Language]] of set theory i.e. $\mathcal{L}=\{ \in \}$
and $M\subseteq N$ (i.e. $M$ is a [[Substructure]] of $N$)
We say that $M$ is a transitive substructure of $N$ if 
for any $x,y\in N$:
$$
y\in M\land xEy \implies x\in M
$$

We will often say $M$ is a transitive model of $T\subseteq ZFC$.
This means that $(N,E)$ is some fixed [[Model]] of $ZFC$,
and $(M,E)$ is a transitive substructure of $(N,E)$ and:
$$
(M,E) \models T
$$
### Lemma
Let $(N,E)$ be a [[Model]] of $ZFC$.
Suppose that $M\in N$ is $E$-[[Foundations/Set Theory/Transitive|Transitive]] i.e. 
$$
(\forall x,y\in N)\, E(y,M) \land E(x,y) \implies E(x,M)
$$
Then $(M,E)$ is a transitive substructure of $N$.
#### Proof
Suppose $y\in M$ and $E(x,y)$.
From $E(x,y)$ we conclude $y\in N$.
By [[Axiom of Separation]] in $N$, we can form the set 
$$
M'=\{ z : E(z,M) \}
$$
By [[Axiom of Extensionality]] in $N$, $M'=M$.
As $y\in M$, it has to be $E(y,M)$.
As $M$ is $E$-[[Foundations/Set Theory/Transitive|Transitive]], we conclude $E(x,M)$

### Lemma
Let $N$ be the set theoretic universe.
If $M$ is transitive in $N$ then $(M,\in)\models$ [[Axiom of Extensionality]] + [[Axiom of Foundation]]
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
[[Axiom of Foundation]]
$$
\Big(\forall x\Big)\,\Big(x\neq \varnothing \implies \big(\exists m\big)\,\big(m\in x\land (\forall w)\,w\not\in m\lor w\not\in x\big)\Big)
$$
Suppose $x\in M$.
Find using [[Axiom of Foundation]] an $\in$-minimal $m\in x$ (in $N$)
By [[Foundations/Set Theory/Transitive|Transitivity]] we get $m\in M$
We can check that $m$ is still $\in$-minimal in $M$.
