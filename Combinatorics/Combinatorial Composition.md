Let $F:\mathcal{B}\to \mathcal{B}_{R}$ and $G:\mathcal{B}\to \mathcal{B}_{R}$ be [[Combinatorial Structure]]s.
We define their composition as:
$$
(G \circ F)(A) = \bigsqcup \Big\{ G\big(\{ \alpha_{1},\alpha_{2},\dots,\alpha_{k} \}\big) : S_{1}\sqcup S_{2}\sqcup\dots \sqcup S_{k} = A;
\, \alpha_{i}\in F(S_{i}) \Big\}
$$
with weight 
$$
w_{G\circ F} = w_{G} \cdot \prod_{i=1}^{k} w_{F}(\alpha_{i})
$$
Note that for this to be well defined, we need $F(\varnothing)=\varnothing$,
otherwise there is infinitely many partitions of $A$.

