Let $G$ be a connected graph and $a\ne b$ are not connected
The minimum size of $a-b$ [[Separator]] is the maximum number 
of disjoint paths from $a$ to $b$.
Equivalently if all $a-b$ separators have size at least $k$ 
then there exist $k$ disjoint paths from $a$ to $b$.
### Proof
#### Setup
Suppose it is not true.
Then it has a counterexample for some $k$, assume $k$ is smallest
Note $k\geq 2$, as the theorem holds for $k=1$
Let $\mathcal{G}$ be the set of counterexamples for that $k$
Let $G\in \mathcal{G}$ be a counterexample with the least number of edges.

For each $a,b$ in $G$, define $\kappa_{a,b}$ to be the size of smallest separator.
Suppose $a,b$ are counterexamples in $G$ 
with a maximum of $k$ disjoint paths from $a$ to $b$
Let $S$ be the minimum $a-b$ separator
Then $\lvert S \rvert=\kappa_{a,b}>k$ 
#### Step 1
There is a minimum separator $\tilde{S}$ which is neither $N(a)$ nor $N(b)$
To prove this, assume WLOG $S=N(a)$
If $N(a)\cap N(b)\neq \emptyset$, then let $x\in N(a)\cap N(b)$
Consider $G'=G-x$
In $G'$ there is at most $k-1$ disjoint paths from $a$ to $b$
(if there was more then in $G$ we can always add back the path $axb$)
By minimality, there is a separator $S'$ of size $k-1$ in $G'$
But then $S=S'\cup \{ x \}$ is a separator in $G$
Hence assume $N(a)\cap N(b)=\emptyset$
Let $ax_{1}x_{2}\dots x_{l}b$ be the shortest path from $a$ to $b$
where $l\geq 2$
As this is the shortest path, we know $x_{2}\not\in N(a)$
Also $x_{2}\ne b$
Now let $G'=G-x_{1}x_{2}$
Now $\kappa_{a,b}(G')<\lvert S \rvert$ otherwise there is a smaller counterexample
So let $S'$ be a separator of $a,b$ in $G'$ with size $\lvert S \rvert-1\geq 1$
Then $S'\cup \{ x_{1} \}$ and $S'\cup \{ x_{2} \}$ are both separators of $a,b$ in $G$
Now note $S'\cup \{ x_{2} \}\ne N(a)$ and $S'\cup \{ x_{1} \}\ne N(b)$
Also if $S'\cup \{ x_{1} \}=N(a)$ and $S'\cup \{ x_{2} \}=N(b)$ 
then $N(a)\cap N(b)=S'\ne \emptyset$
And thus we found a separator of $a,b$ that is neither $N()$




## Corollary
Let $G$ be connected with $\lvert G \rvert\geq 2$
Then $G$ is $k$-connected if and only if all pairs of $a\ne b$
admit $k$ disjoint paths from $a$ to $b$.
