Let $G$ be a [[Group]] and $Syl_{p}(G)$ the set of [[Sylow Subgroup]]s.
Then all elements of $Syl_p(G)$ are [[Conjugate]].
#### Proof
We prove a stronger statement (DONT NEED TO). 
Suppose $P\in Syl_p(G)$ and $Q\leq G$ is a $p$-subgroup. 
Then $Q\leq gPg^{-1}$ for some $g\in G$. 
Consider the [[Group Action]] of $Q$ 
on left cosets of $G/P$ by left multiplication. 
Note that $|G/P|=m$, 
so there is at least one [[Orbit]] not divisible by $p$. 
But all orbits divide $|Q|$, so there is an orbit of size $1$. 
So for some $g\in G$, and every $q\in Q$ 
we have $qgP=gP$ 
i.e. $g^{-1}qg\in P$. 
Hence for some $g\in G$ we have $Q\leq gPg^{-1}$. 