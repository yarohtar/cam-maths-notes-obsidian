Let $\mathcal{C}$ and $\mathcal{D}$ be [[Category]]
Let $F,G$ be [[Functor]]s $\mathcal{C}\xrightarrow{F,G}\mathcal{D}$
Let $\alpha:F\to G$ be a [[Natural Transformation]]
and suppose $\alpha$ is an [[Isomorphism]] in the [[Category of Functors]] $[\mathcal{C},\mathcal{D}]$.
Then $\alpha$ is called a natural isomorphism.
### Lemma
Let $F,G:\mathcal{C}\to \mathcal{D}$ be [[Functor]]s
Let $\alpha:F\to G$ be a [[Natural Transformation]] between them.
Then $\alpha$ is an [[Isomorphism]] in [[Category of Functors]] $[\mathcal{C}, \mathcal{D}]$ 
if and only if 
each $\alpha_{A}$ is an [[Isomorphism]] in $\mathcal{D}$
#### Proof
##### $\implies$
Obvious since composition in $[\mathcal{C},\mathcal{D}]$ is pointwise.
##### $\impliedby$
Suppose each $\alpha_{A}$ has an inverse $\beta_{A}$ 
We need to verify naturality of $\beta$.
Given $A\xrightarrow{f}B$ in $\mathcal{C}$, consider:
```tikz
\usepackage{tikz-cd}

\begin{document}
\begin{tikzcd}
GA 
\arrow[r,"Gf"] 
\arrow[d,shift left, "\beta_{A}"] 
& GB
\arrow[d,shift left, "\beta_{B}"]
\\
FA
\arrow[u,shift left,"\alpha_{A}"]
\arrow[r,"Ff"] 
& FB 
\arrow[u,shift left, "\alpha_{B}"]
\end{tikzcd}
\end{document}
```
We have 
$$
\beta_{B}(Gf)=\beta_{B}(Gf)\alpha_{A}\beta_{A}=\beta_{B}\alpha_{B}(Ff)\beta_{A}=(Ff)\beta_{A}
$$ 