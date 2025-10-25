Let $A$ be an [[Object]] of a [[Locally Small]] [[Category]] $\mathcal{C}$ 
and let $F:\mathcal{C}\to \mathrm{Set}$ be a [[Functor]] to [[Category of Sets]]
Then there is a bijection between
[[Natural Transformation]]s $\mathcal{C}(A,\cdot)\to F$ (where $\mathcal{C}(A,\cdot)$ is [[Hom-Functor]])
and elements of $FA$.
Moreover, the bijection is a [[Natural Transformation]] in $A$ and $F$.
### Proof
Given $\alpha:\mathcal{C}(A,\cdot)\to F$ a [[Natural Transformation]]
Note that $\mathcal{C}(A,A)\xrightarrow{\alpha_{A}}FA$
so define $\Phi(\alpha)=\alpha_{A}(1_{A})\in FA$
Given $x\in FA$ 
we define a [[Natural Transformation]] $\Psi(x):\mathcal{C}(A,\cdot)\to F$ by
$$
\begin{align}
\Psi(x)_{B} : \mathcal{C}(A,B) & \to FB \\
(A\xrightarrow{f}B)  & \to(Ff)(x)
\end{align}
$$
Naturality of $\Psi(x)$ follows from [[Functor|functoriality]] of $F$.
We know 
$$
\Phi\Psi(x) = \Psi(x)_{A}(1_{A}) = F(1_{A})(x)=x
$$
And for all $B$ and $f$

```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
C(A,A) \arrow[r,"C(A,f)"] \arrow[d,"\alpha_{A}"]
 & C(A,B) \arrow[d,"\alpha_{B}"] \\
FA \arrow[r,"f"]
 & FB
\end{tikzcd}
\end{document}
```

**
$$
\Psi(\Phi(\alpha))_{B}(A\xrightarrow{f}B)=(Ff)(\Phi(\alpha))=(Ff)\alpha_{A}(1_{A})=\alpha_{B}\mathcal{C}(A,f)(1_{A})=\alpha_{B}(f)
$$
So $\Phi$ and $\Psi$ are inverse bijections.


