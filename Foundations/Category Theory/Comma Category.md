Let $\mathcal{A}$, $\mathcal{B}$ and $\mathcal{C}$ be [[Category|Categories]]
Let $P:\mathcal{A}\to \mathcal{C}$ and $Q:\mathcal{B}\to \mathcal{C}$
The comma category, written as $(P\downarrow Q)$ 
is the category defined as follows
1. Objects are triples $(A,h,B)$ with $A\in \operatorname{ob}\mathcal{A}$, $B\in \operatorname{ob}\mathcal{B}$ and $h:P(A)\to Q(B)$
2. maps $(A,h,B)\to(A',h',B')$ are pairs $(f:A\to A',g:B\to B')$ 
   such that we have a [[Commutative Diagram]]
```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
P(A) \arrow[r,"P(f)"] \arrow[d,"h"]
 & P(A') \arrow[d,"h'"] \\
Q(B) \arrow[r,"Q(g)"]
 & Q(B')
\end{tikzcd}
\end{document}
```
### Special case
Let $G:\mathcal{D}\to \mathcal{C}$ be a [[Functor]].
Let also $A:1\to \mathcal{C}$ be the functor from the trivial category to $\mathcal{C}$,
sending the only element of $1$ to the object $A\in \operatorname{ob}\mathcal{C}$ (by abuse of notation)
We write $(A,G)$ for their comma category.
This category has
1. [[Object]]s as pairs $(B,h)$ for $B\in \operatorname{ob}\mathcal{D}$ and $h:GB\to A$
2. [[Morphism]]s $(B,h)\to(B',h')$ as morphisms $f:B\to B'$
   such that we have a [[Commutative Diagram]]
```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
GB \arrow[r, "Gf"] \arrow[dr, "h"] 
& GB' \arrow[d, "h'"] \\
A
\end{tikzcd}
\end{document}
```
