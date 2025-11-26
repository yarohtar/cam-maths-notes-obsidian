---
aliases:
  - Dense
---
Let $(\mathbb{P},\leq,\mathbb{1})$ be a [[Forcing Partial Order]] 
Let $D\subseteq \mathbb{P}$
We say that $D$ is dense below $p$ if 
$$
(\forall q\leq p)\, (\exists r\leq q)\, r\in D
$$
Also $D$ is [[Dense]] if it is dense below any $p$ (i.e. dense below $\mathbb{1}$).
### Lemma
If $E\subseteq \mathbb{P}$ is dense below $p$ and $q\leq p$
then $E$ is dense below $q$.
### Lemma
If $E\subseteq \mathbb{P}$ such that 
$$
\{ r : E \text{ is dense below }r \}
$$
is dense below $p$, then $E$ is dense below $p$.
### Lemma
Let $G$ be a $\mathbb{P}$-[[Generic Filter]] over a countable [[Transitive Model]] $M$.
Let $E\subseteq \mathbb{P}$ and $E\in M$.
Then either $G\cap E\neq \varnothing$ or 
$$
(\exists q\in G)\, (\forall r\in E)\, r\operatorname{\bot}q
$$
Furthermore, if $p\in G$ and $E$ is dense below $p$ then 
$$
G\cap E\neq \varnothing
$$

