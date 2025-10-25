Suppose a [[Functor]] $F:\mathcal{C}\to \mathrm{Set}$ is [[Representable]].
Then $F$ is [[Isomorphic]] to some $\mathcal{C}(A,\cdot)$.
By the [[Yoneda Lemma]], there is some $x\in FA$ 
such that $\Psi(x)$ is a [[Natural Isomorphism]] $\mathcal{C}(A,\cdot)\to F$
We call $(A,x)$ the representation of $F$.
We call $x$ a [[Universal Element]] of $F$
### Corollary
If $(A,x)$ and $(B,y)$ are both representations of $F:\mathcal{C}\to \mathrm{Set}$ 
then there is a unique [[Isomorphism]] $A\xrightarrow{f}B$ in $\mathcal{C}$ such that $(Ff)(x)=y$.
#### Proof
Fix an [[Object]] $C\in \operatorname{ob}(\mathcal{C})$.
Let $f:A\to B$.
Let $\mathcal{C}(f,\cdot):\mathcal{C}(B,\cdot)\to \mathcal{C}(A,\cdot)$ be its image under the [[Yoneda Embedding]]
and consider the function $\mathcal{C}(f,C):\mathcal{C}(B,C)\to \mathcal{C}(A,C)$ 
defined by:
$$
(B\xrightarrow{g}C)\to(A\xrightarrow{gf}C)
$$
Also let $\Psi^{A}$ be the bijection between elements of $FA$
and [[Natural Transformation]]s $\mathcal{C}(A,\cdot)\to F$ given by [[Yoneda Lemma]]
Now $\Psi^{A}(x)_{C}:\mathcal{C}(A,C)\to FC$ 
is a function given by:
$$
(A\xrightarrow{g}C)\to(Fg)(x)
$$
and similarly $\Psi^{B}(y)_{C}:\mathcal{C}(B,C)\to FC$
is a function given by:
$$
(B\xrightarrow{g}C)\to(Fg)(y)
$$
Consider the diagram
```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
\mathcal{C}(B,C) \arrow[]
\end{tikzcd}
\end{document}
```


Thus let $C=B$ and $g=f$ to find 
$$
\Psi^{A}(x)_{B}(f) = (Ff)(x) = y
$$


Similarly, $\Psi^{B}(y):\mathcal{C}(B,\cdot)\to F$
is sending $C\in \mathcal{C}$
to a mapping $\mathcal{C}(B,C)\to FC$ given by $(B\xrightarrow{g}C)\to(Fg)(y)$

The [[Epimorphism]] $Ff(x)=y$ is equivalent to saying that
```tikz
\usepackage{tikz-cd}

\begin{document}
\begin{tikzcd}
\mathcal{C}(B,\cdot) \arrow[rr,"\mathcal{C}(f{,}\cdot)"] \arrow[dr,swap,"\Psi(y)"] 
&&
\mathcal{C}(A,\cdot) \arrow[dl,"\Psi(x)"] \\
& F
\end{tikzcd}
\end{document}
```
commutes.
So $f$ must be the unique [[Isomorphism]] in $\mathcal{C}$ 
whose image under the [[Yoneda Embedding]] is $\Psi(x)^{-1}\Psi(y)$
