Suppose a [[Functor]] $F:\mathcal{C}\to \mathrm{Set}$ is [[Representable]].
Then $F$ is [[Isomorphic]] to some $\mathcal{C}(A,\cdot)$.
By the [[Yoneda Lemma]], there is some $x\in FA$ 
such that $\Psi(x)$ is a [[Natural Isomorphism]] $\mathcal{C}(A,\cdot)\to F$
We call $x$ a [[Universal Element]] of $F$
### Corollary
If $(A,x)$ and $(B,y)$ are both representations of $F:\mathcal{C}\to \mathrm{Set}$ 
then there is a unique [[Isomorphism]] $A\xrightarrow{f}B$ in $\mathcal{C}$ such that $Ff(x)=y$.
#### Proof

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
