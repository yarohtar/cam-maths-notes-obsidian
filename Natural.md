Let $\mathcal{A}_{X}$ and $\mathcal{B}_{X}$ be two types indexed by [[Object]]s $X$ of some [[Category]] $\mathcal{C}$
along with types $\mathcal{A}_{f}:\mathcal{A}_{X}\to \mathcal{A}_{Y}$ and $\mathcal{B}_{f}:\mathcal{B}_{X}\to \mathcal{B}_{Y}$ 
along with classes of assignments $\mathcal{A}_{f}:\mathcal{A}_{X}\to \mathcal{A}_{Y}$
and $\mathcal{B}_{f}:\mathcal{B}_{X}\to \mathcal{B}_{Y}$ for any [[Morphism]] $f:X\to Y$.
An assignment $\eta_{X}:\mathcal{A}_{X}\to \mathcal{B}_{X}$ is natural in $X$ if for any $f:X\to Y$ in $\mathcal{C}$
we have a [[Commutative Diagram]]
```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
\mathcal{A}_{X} \arrow[r, "\mathcal{A}_{f}"] 
\arrow[d, "\eta_{X}"] 
& \mathcal{A}_{Y} \arrow[d, "\eta_{Y}"]\\
\mathcal{B}_{X} \arrow[r, "\mathcal{B}_{f}"] 
& \mathcal{B}_{Y}
\end{tikzcd}
\end{document}
```
i.e. for any $A\in \mathcal{A}_{X}$ we have 
$$
\eta_{Y}(\mathcal{A}_{f}(A)) = \mathcal{B}_{f}(\eta_{X}(A))
$$
