Suppose a [[Functor]] $F:\mathcal{C}\to \mathrm{Set}$ is [[Representable]].
Then $F$ is [[Isomorphic]] to some $\mathcal{C}(A,\cdot)$.
By the [[Yoneda Lemma]], there is some $x\in FA$ 
such that $\Psi(x)$ is a [[Natural Isomorphism]] $\mathcal{C}(A,\cdot)\to F$
We call $x$ a [[Universal Element]] of $F$
### Corollary
If $(A,x)$ and $(B,y)$ are both representations of $F:\mathcal{C}\to \mathrm{Set}$ 
then there is a unique [[Isomorphism]] $A\xrightarrow{f}B$ in $\mathcal{C}$ such that $Ff(x)=y$.
#### Proof
Let $f:A\to B$.
Let $\mathcal{C}(f,\cdot):\mathcal{C}(B,\cdot)\to \mathcal{C}(A,\cdot)$ be its image under the [[Yoneda Embedding]]
Also let $\Psi^{A}$ be the bijection between elements of $FA$
and [[Natural Transformation]]s $\mathcal{C}(A,\cdot)\to F$ given by [[Yoneda Lemma]]
and similarly $\Psi^{B}$.
Now $\Psi^{A}(x):\mathcal{C}(A,\cdot)\to F$ 
is sending [[Object]] $C\in \mathcal{C}$ 
to a mapping $\mathcal{C}(A,C)\to FC$ given by $(A\xrightarrow{g}C)\to(Fg)(x)$

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
