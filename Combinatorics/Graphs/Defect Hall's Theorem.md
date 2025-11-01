Let [[Simple Graph|Graph]] $G=(X\sqcup Y,E)$ be bipartite. 
Then $G$ contains a [[Matching with Deficiency]] $d$ 
if and only if $\lvert A \rvert \leq \lvert N(A) \rvert+d$ for all $A\subseteq X$
### Proof
Forward direction is easy
Now apply [[Hall's Theorem]] on graph:
$$
G'=(X\sqcup(Y\cup \{ z_{1},\dots,z_{d} \}), E\cup E')
$$
where
$$
E'=\{ xz_{i} : x\in X, 1\leq i\leq d \}
$$
After finding the [[Matching]], remove the vertices $z_{1},\dots,z_{d}$
Because of injectivity, we get a [[Matching with Deficiency]] at most $d$
Then remove a few edges to get deficiency $d$
