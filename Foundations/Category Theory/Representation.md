Suppose a [[Functor]] $F:\mathcal{C}\to \mathrm{Set}$ is [[Representable]].
Then $F$ is [[Isomorphic]] to some $\mathcal{C}(A,-)$.
We say that $(A,\alpha)$ is a representation of $F$
where $\alpha$ is a [[Natural Isomorphism]]
$$
\alpha:\mathcal{C}(A,-) \to F
$$



By the [[Yoneda Lemma]], there is some $x\in FA$ 
such that $\Psi(x)$ is a [[Natural Isomorphism]] $\mathcal{C}(A,-)\to F$
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
and [[Natural Transformation]]s $\mathcal{C}(A,\cdot)\to F$ given by [[Yoneda Lemma]].
In particular $\Psi^{A}(x)$ is a [[Natural Isomorphism]].
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
\mathcal{C}(B,C) \arrow[rr, "\mathcal{C}(f{,}C)"] \arrow[dr, swap, "\Psi^{B}(y)_{C}"]
&& \mathcal{C}(A,C) \arrow[dl, "\Psi^{A}(x)_{C}"] \\
& FC
\end{tikzcd}
\end{document}
```

This is a [[Commutative Diagram]]
if and only if
for any $B\xrightarrow{g}C$ we have:
$$
(Fgf)(x) = (Fg)(y)
$$
Thus if $f$ is such that $f(x)=y$ then this diagram commutes for any $C$.
But then the following is also a [[Commutative Diagram]]
(of [[Natural Transformation]]s in $[\mathcal{C},\mathrm{Set}]$) 
```tikz
\usepackage{tikz-cd}

\begin{document}
\begin{tikzcd}
\mathcal{C}(B,\cdot) \arrow[rr,"\mathcal{C}(f{,}\cdot)"] \arrow[dr,swap,"\Psi^{B}(y)"] 
&&
\mathcal{C}(A,\cdot) \arrow[dl,"\Psi^{A}(x)"] \\
& F
\end{tikzcd}
\end{document}
```
So if $f(x)=y$ then it has to be that $\mathcal{C}(f,\cdot)=\Psi^{A}(x)^{-1}\Psi^{B}(y)$.
But [[Yoneda Embedding]] is [[Faithfull]] so $f$ is unique.

Also [[Yoneda Embedding]] is [[Full]] so there is some $f$ such that 
$$
\mathcal{C}(f,\cdot) = \Psi^{A}(x)^{-1}\Psi^{B}(y)
$$
which then implies that for any $C$ and $B\xrightarrow{g}C$:
$$
(Fgf)(x)=(Fg)(y)
$$
i.e. we have to have $(Ff)(x)=y$
It is also [[Isomorphic]], as $\Psi^{A}(x)$ and $\Psi^{B}(y)$ are [[Natural Isomorphism]]s,
so
$$
\mathcal{C}(f,\cdot)^{-1}=\mathcal{C}(f^{-1},\cdot)=\Psi^{B}(y)^{-1}\Psi^{A}(x)
$$


