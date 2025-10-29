Let $D:J\to \mathcal{C}$ be a [[Diagram]].
A cone over $D$ consists of an [[Object]] $A$ of $\mathcal{C}$ (apox)
together with [[Morphism]]s $\lambda_{j}:A\to D(j)$ for all $j\in \operatorname{ob}J$ (legs)
satisfying $D(x)\lambda_{j}=\lambda_{j'}$ for all $\alpha:j\to j'$ in $J$
```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
& & A \arrow[ddrr] \arrow[ddr] \arrow[dd] \arrow[ddl]\arrow[ddll]\\
\\
\cdot & \cdot & \cdot & \cdot & \cdot
\end{tikzcd}
\end{document}
```
A morphism of cones $(A,(\lambda_{j}:j\in \operatorname{ob}J))\to(B,(\mu_{j}:j\in \operatorname{ob}J))$
is a morphism $f:A\to B$ satisfying $\mu_{j}f=\lambda_{j}$ for all $j$ 
We write $\operatorname{Cone}(D)$ for the category of cones over $D$.
