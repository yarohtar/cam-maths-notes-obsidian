Let $G$ be a [[Group]].
The set of [[Sylow Subgroup]]s $Syl_p(G)$ is nonempty.
#### Proof
Consider $\Omega$, the set of all subsets of $G$ of size $p^a$. 
Note that $|\Omega|={p^am\choose p^a}$ which is not divisible by $p$. 
Consider the natural (left multiplication) [[Group Action]] of $G$ on $\Omega$.
It has at least one [[Orbit]] not divisible by $p$.
Suppose that is the orbit of $X\subseteq G$. 
Now $|G_X|\cdot |Orb_G(X)|=|G|$ by [[Orbit-Stabilizer Theorem]] 
so $p^a\mid |G_X|$
so $|G_X|\geq p^a$. 
But also $|G|\leq |Orb_G(X)|\cdot |X|$ 
because $G=\bigcup_{g\in G} g(X)=\bigcup_{Y\in Orb_G(X)}Y$.  
So $|G_X|\leq p^a$ 
so $|G_X|=p^a$. 