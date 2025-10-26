An [[Object]] $P$ of a [[Locally Small]] [[Category]] $\mathcal{C}$ is projective
if [[Hom-Functor]] $\mathcal{C}(P,-)$ preserves [[Epimorphism]]s
i.e. if given
```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
& P 
\arrow[d,"f"]\\
Q \arrow[r,two heads,"g"] & R
\end{tikzcd}
\end{document}
```
there exists $h:P\to Q$ with $gh=f$

