Let $S\subseteq L$, $t\in L$. If $S\models t$ then $S\vdash t$.
#### Proof
Since $S\models t$, we have $S\cup \{ \neg t \}\models \bot$
By [[Model existence lemma]] $S\cup \{ \neg t \}\vdash \bot$ and hence $S\vdash \neg t$ by the [[Deduction Theorem (Propositional Logic)|Deduction Theorem]].
Add the lines:
$$
\begin{align}
\neg \neg t\implies t\quad %quad
\quad %quad
 & \text{(A3)} \\
t\quad %quad
\quad %quad
 & \text{(MP)}
\end{align}
$$
To get $S\vdash t$

