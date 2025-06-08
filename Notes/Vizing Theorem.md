Let $G$ be a graph with $\Delta(G)=\Delta$
Then $\chi'(G)=\Delta$ or $\chi'(G)=\Delta+1$
### Proof
Clearly $\chi'(G)\geq \Delta$
WTS $\chi'(G)\leq \Delta+1$
Induction on edges
Pick an edge $xy_{1}$ and colour everything else in $\Delta+1$
Construct the longest sequence of distinct $y_{1}y_{2}\dots y_{k}$
where if $y_{i}$ is missing colour $c_i$ then $xy_{i+1}$ is coloured $c_{i}$
#### Case 1
No $y$ such that $xy$ is coloured $c_{k}$
Note $k\leq \Delta$
Now recolour $y_{i}$ with colour $c_{i}$
#### Case 2
$c_{k}=c_{j}$ for some $j<k$
Recolour $y_{i}$ with $c_{i}$ for $1\leq i<j$
leaving $y_{j}$ uncoloured, so WLOG $j=1$
