Let $S\subseteq L$. Then if $S$ is [[Inconsistency|consistent]], then $S$ has a model. 
#### Proof
We only consider the case when the set $P$ of primitive propositions is countable. We will do the general case in chapter 3

Note that $L_{1}=P\cup \{ \bot \}$ is countable, and hence by induction $L_{n}$ is also countable for all $n\in \mathbb{N}$. Thus $L=\bigcup_{n\in \mathbb{N}}L_{n}$ is countable.
We enumerate $L$ as $t_{1},t_{2},\dots$

If $T\subseteq L$ is consistent and $t\in L$ then one of $T\cup \{ t \}$ or $T\cup \{ \neg t \}$ is consistent. Indeed, if not, then $T\cup \{ t \}\vdash \bot$ and $T\cup \{ \neg t \}\vdash \bot$
Then by [[Deduction Theorem]], we have $T\vdash \neg t$ and $T\vdash(\neg t\implies \bot)$ and hence $T\vdash \bot$ by (MP) which is a contradiction

Now start with the consistent $S$. 
Let $S_{0}=S$
We define sets $S_{n}$ by induction:
Assume $S_{n-1}$ is defined and is consistent
Then let $S_{n}$ be either $S_{n-1}\cup \{ t_{n} \}$ or $S_{n}$

