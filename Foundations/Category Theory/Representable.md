We say a [[Functor]] $F:\mathcal{C}\to \mathrm{Set}$ is representable 
if it's [[Isomorphic]] to $\mathcal{C}(A,\cdot)$ for some $A$,
i.e. there is some [[Natural Isomorphism]] $\mathcal{C}(A,\cdot)\to F$

### Examples
The forgetful functor $F:\mathrm{Gp}\to \mathrm{Set}$ 
is representable with [[Representation]] $(\mathbb{Z},1)$.
That is, for any [[Group]]s $G,H\in \operatorname{ob}\mathrm{Gp}$
with a [[Homomorphism]] $f:G\to H$ 
we can have a [[Natural Isomorphism]] $\alpha$
and a [[Commutative Diagram]]
```tikz
\usepackage{tikz-cd}
\usepackage{amssymb}
\begin{document}
\begin{tikzcd}
\mathcal{C}(\mathbb{Z},G) \arrow[r,"\mathcal{C}(\mathbb{Z}{,}f)"] \arrow[d,"\alpha_{G}"]
 & \mathcal{C}(\mathbb{Z},H) \arrow[d,"\alpha_{H}"] \\
FG \arrow[r,"Ff"]
 & FH
\end{tikzcd}
\end{document}
```
where $\alpha_{G}$ sends a [[Homomorphism]] $g:\mathbb{Z}\to G$
to the element $g(1)$



