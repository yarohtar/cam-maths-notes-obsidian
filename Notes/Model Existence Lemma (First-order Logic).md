Let $S$ be a consistent theory in a first-order language $L=L\left( \Omega,\prod \right)$. Then $S$ has a model.

#### Idea
We build a model from the language itself 
To begin with, we let $A$ be the set of closed terms of $L$, i.e. terms with no variables
We turn this into a [[Structure]] in the obvious way

$A$ is still not a model (e.g. $1+0$ and $1$ are not equal in $A$)
Define equivalence relation $\sim$ on $A$ by 
$s\sim t$ iff $T\vdash(s=t)$ where($s,t \in A$)
Replace $A$ with $A /_{\sim}$
Two issues remain

Firstly, in general, $T$ is not complete (i.e. there are sentences $p$ where neither $T\vdash p$ nor $T\vdash \neg p$)
Remedy: Given consistent theory $S$ there is a consistent, complete $\bar{S}\supseteq S$

Secondly, we are missing some elements that are guaranteed by $(\exists x)p$ whre $p$ is for example $x\cdot x=1+1$
Remedy: We add a witness, i.e. a new constant $c$ to $L$ (the new language is $L'=L\left( \Omega \cup \{ c \},\prod \right)$) and a new sentence to $T$ to obtain $T'=T\cup \{ p[c /x] \}$

#### Proof (NONEXAMINABLE)
We start with two observations
1. Let $S$ be a consistent theory, $p$ be a sentence
   Then one of $S\cup \{ p \}$ and $S\cup \{ \neg p \}$ is consistent
   If not, then by [[Deduction Theorem (First-order Logic)]] 
   $S\vdash \neg p$ and $S\vdash \neg \neg p$ and hence $S\vdash \bot$ by (MP)
   By [[Zorn's Lemma]] there is a maximal consistent theory $\bar{S}\supseteq S$. 
   Then for every sentence $p$, either $p \in \bar{S}$ or $\neg p \in \bar{S}$
   In particular $\bar{S}$ is complete
2. 
