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
Then either $G\cap E\neq \varnothing$ or some $q\in G$ has:
$$
(\forall r\in E)\ r\operatorname{\bot}q
$$
Furthermore, if $p\in G$ and $E$ is dense below $p$ then 
$$
G\cap E\neq \varnothing
$$
#### Proof
Let 
$$
D=\{ p\in \mathbb{P}: (\exists e\in E)\ p\leq e \} \cup \{ p\in \mathbb{P} : (\forall e\in E)\ p\operatorname{\bot}e \}
$$
Then $D$ is dense: let $p\in \mathbb{P}$ and assume $p\not\in D$ 
so that $p$ is compatible with some $e\in E$. 
Then some $r\in \mathbb{P}$ has $r\leq p,e$ so $r\in D$ and $D$ is dense.
Thus $G$ intersects $D$ and let $q\in G\cap D$. 
If $q\leq e$ for some $e\in E$ then $e\in G\cap E$. 
Otherwise, $q$ is incompatible with all elements of $E$ as desired.

To see the last part, note that if $p\in G$ and $E$ is dense below $p$, 
then 


