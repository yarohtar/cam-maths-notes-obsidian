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
Then let $S_{n}$ be either $S_{n-1}\cup \{ t_{n} \}$ or $S_{n-1}\cup \{ \neg t_{n} \}$, so that $S_{n}$ is consistent 
Finally, let $\bar{S}=\bigcup_{n\geq 0}S_{n}$

Note that $S\subseteq \bar{S}$ and $\forall t\in L$ either $t\in \bar{S}$ or $\neg t\in \bar{S}$.

Also $\bar{S}$ is consistent: if $\bar{S}\vdash \bot$ then as proofs are finite, there is some $n$ such that $S_{n}\vdash \bot$ which is a contradiction.

$\bar{S}$ is deductively closed i.e. if $t\in L$ and $\bar{S}\vdash t$ then $t\in \bar{S}$.
Indeed, if $t\not\in \bar{S}$ then $\neg t\in \bar{S}$. So we have a proof:
First write down a proof of $t$ from $S$ and add the lines:
$$
\begin{align}
\neg t\quad %quad
\quad %quad
 & \text{(premiss)} \\
\bot \quad %quad
\quad %quad
 & \text{(MP)}
\end{align}
$$
We now define $v:L\to \{ 0,1 \}$ by
$$
v(t)=\begin{cases}
1  & \text{if } \bar{S}\vdash t \ (\text{i.e. }t\in \bar{S}) \\
0 & \text{otherwise}
\end{cases}
$$
Note that $v$ is a model of $\bar{S}$ and hence of $S$.

We show that $v$ is a valuation:
Firstly, $v(\bot)=0$ since $\bar{S}$ is consistent.
We now check $v(p \implies q)$ for arbitrary $p,q\in L$
##### Case 1
$v(p)=1,v(q)=0$, i.e. $p \in \bar{S}, q\not\in \bar{S}$
need $v(p \implies q)=0$
If not, then $\bar{S}\vdash(p \implies q)$. Write down a proof of $p \implies q$ from $\bar{S}$ and add:
$$
\begin{align}
p \quad %quad
\quad %quad
& \text{(premiss)} \\
q \quad %quad
\quad %quad
 & \text{(MP)}
\end{align}
$$
So $\bar{S}\vdash q$ and $q\in \bar{S}$, since $\bar{S}$ is deductively closed.
##### Case 2
$v(q)=1$ i.e. $q\in \bar{S}$. 
need $v(p \implies q)=1$
Note that
$$
\begin{align}
q \implies (p \implies q)\quad %quad
\quad %quad  \\
&  \text{(A1)} \\
q \quad %quad
\quad %quad
 & \text{(premiss)} \\
p \implies q\quad %quad
\quad %quad
 & \text{(MP)}
\end{align}
$$
So $\bar{S}\vdash(p \implies q)$ and $v(p \implies q)=1$
##### Case 3
$v(p)=0$ i.e. $p\not\in \bar{S}$ and so $\neg p \in \bar{S}$
need: $v(p \implies q)=1$, i.e. $\bar{S}\vdash(p \implies q)$ or equivalently $\bar{S}\cup \{ p \}\vdash q$ by [[Deduction Theorem]]
Note that:
$$
\begin{align}
p\quad %quad
\quad %quad
 & \text{(premiss)}  \\
\neg p\quad %quad
\quad %quad
 & \text{(premiss)} \\
\bot \quad %quad
\quad %quad
 & \text{(MP)} \\
\bot \implies((q\implies \bot)\implies \bot)\quad %quad
\quad %quad
 & \text{(A1)} \\
\neg \neg q\quad %quad
\quad %quad
 & \text{(MP)} \\
\neg \neg q\implies q\quad %quad
\quad %quad
 & \text{(A3)} \\
q\quad %quad
\quad %quad
 & \text{(MP)}
\end{align}
$$

