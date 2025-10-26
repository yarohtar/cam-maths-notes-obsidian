Let $\mathcal{C}$ be a [[Category]] and $A,B\in \operatorname{ob}\mathcal{C}$
A product of $A$ and $B$ is an [[Object]] $A\times B$
together with [[Morphism]]s $\pi_{1}:A\times B\to A$ and $\pi_{2}:A\times B\to B$
with the universal property that 
for any $X$ with maps $p_{1}:X\to A$ and $p_{2}:X\to B$
there exists a unique $f:X\to A\times B$
such that we have a [[Commutative Diagram]]
```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
& X \arrow[dddl, swap, "p_{1}"] 
\arrow[dd,"f"]
\arrow[dddr, "p_{2}"] \\
\\
& A\times B \arrow[dl, "\pi_{1}"]
\arrow[dr, swap, "\pi_{2}"] \\
A & & B

\end{tikzcd}
\end{document}
```

When $\mathcal{C}$ is [[Locally Small]], we can define a [[Functor]] $F:\mathcal{C}\to \mathrm{Set}$
defined by
$$
FC = \mathcal{C}(C,A) \times \mathcal{C}(C,B)
$$
If this is [[Representable]], let $(P,\alpha)$ be its [[Representation]].
i.e. $\alpha:\mathcal{C}(P,-)\to F$ is a [[Natural Isomorphism]]
Note that $\alpha_{P}(1_{P})\in \mathcal{C}(P,A)\times \mathcal{C}(P,B)$ is the [[Universal Element]],
consisting of $(\pi_{1},\pi_{2})$ where $\pi_{1}:P\to A$ and $\pi_{2}:P\to B$
and thus $P$ is the product of $A$ and $B$. 

