Let $G=(X\sqcup Y,E)$ be bipartite. 
There exists a [[Matching]] from $X$ to $Y$ if and only if 
for all $A\subseteq X$, $\lvert A \rvert\leq \lvert N(A) \rvert$
## Proof
If there is a matching, we can find an injection from $A$ to $N(A)$

Now suppose $\lvert A \rvert\leq \lvert N(A) \rvert$ for all $A\subseteq X$
We go by induction on $\lvert X \rvert$
### Case 1
Suppose there is some $\emptyset \ne A\neq X$ such that $\lvert A \rvert=\lvert N(A) \rvert$
Then $A$ satisfies the criterion so there is a matching on $A$
Also set $B\subseteq X\setminus A$
Write:
$$
\lvert A \rvert +\lvert B \rvert \leq \lvert N_{G}(A\cup B) \rvert = \lvert N_{G}(A) \rvert  + \lvert N_{G_{2}}(B) \rvert  
$$
