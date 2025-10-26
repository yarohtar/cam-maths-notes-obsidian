Let $A$ be an [[Object]] of a [[Locally Small]] [[Category]] $\mathcal{C}$.
Let $\mathcal{C}(A,-)$ be a [[Hom-Functor]] $\mathcal{C}\to \mathrm{Set}$.
and let $F:\mathcal{C}\to \mathrm{Set}$ be a [[Functor]] to [[Category of Sets]].
These are objects in the [[Category of Functors]] $[\mathcal{C},\mathrm{Set}]$.

Yoneda lemma says that the set of [[Natural Transformation]]s $\mathcal{C}(A,-)\to F$
is [[Isomorphic]] to $FA$:
$$
[\mathcal{C},\mathrm{Set}](\mathcal{C}(A,-),F) \cong FA
$$
Moreover, this [[Isomorphism]] is natural in both $A$ and $F$ i.e.
given the functors
$$
\begin{align}
[\mathcal{C},\mathrm{Set}](\mathcal{C}(\bullet_{1},-), \bullet_{2})  & : \mathcal{C}\times[\mathcal{C},\mathrm{Set}] \to \mathrm{Set} \\
\bullet_{2}\bullet_{1}  & : \mathcal{C}\times[\mathcal{C},\mathrm{Set}] \to \mathrm{Set}
\end{align}
$$
there is a [[Natural Isomorphism]] between them.
This [[Natural Isomorphism]] is given by:
$$
\begin{align}
\Phi_{(A,F)}: [\mathcal{C},\mathrm{Set}](\mathcal{C}(A,-), F)  & \to FA  \\
\alpha & \to \alpha_{A}(1_{A})
\end{align}
$$
and its inverse is given by:
$$
\begin{align}
\Psi_{(A,F)}: FA &  \to [\mathcal{C},\mathrm{Set}](\mathcal{C}(A,-),F) \\
x & \to \left(\mathcal{C}(A,-)\xrightarrow{\alpha}F\right) \\
\end{align}
$$
where
$$
\alpha_{B}(A\xrightarrow{f}B)=(Ff)(x)
$$
### what is actually written here?
In a way, given $A$ from $\mathcal{C}$ and $F$ from $[\mathcal{C},\mathrm{Set}]$,
there is only two ways to make a set out of them.
The obvious one is $FA$.
The other way is the set of [[Natural Transformation]]s from $\mathcal{C}(A,-)$ to $F$.
Yoneda says that these two ways are the same "in a natural way".

Suppose that for a [[Functor]] $F:\mathcal{C}\to \mathrm{Set}$ we could define a functor
$$
F'=[\mathcal{C},\mathrm{Set}](\mathcal{C}(\bullet,-),F)
$$
which is also $F':\mathcal{C}\to \mathrm{Set}$ 
(i.e. it takes $A\in \operatorname{ob}\mathcal{C}$ and gives us the set $[\mathcal{C},\mathrm{Set}](\mathcal{C}(A,-),F)$)
Then we could define $F'',F''',\dots$
Yoneda lemma says that there are [[Natural Isomorphism]]s between these,
so we don't need to worry about the infinite tower.
### Proof
Firstly, fix $(A,F)$ and call $\Phi=\Phi_{(A,F)}$ and $\Psi=\Psi_{(A,F)}$.
We need to prove:
$$
\Phi \Psi=1_{FA}
$$
and
$$
\Psi \Phi = 1_{[\mathcal{C},\mathrm{Set}](\mathcal{C}(A,-),F)}
$$
Firstly, let $x\in FA$:
$$
\begin{gather}
\Phi(\Psi(x)) = \Psi(x)_{A}(1_{A}) = (F 1_{A})(x) = 1_{FA}(x)
\end{gather}
$$
Now let $\alpha:\mathcal{C}(A,-)\to F$ be a [[Natural Transformation]].
$$
\Psi(\Phi(\alpha))=\Psi(\alpha_{A}(1_{A}))
$$
For any [[Morphism]] $A\xrightarrow{f}B$ in $\mathcal{C}$ we have:
$$
\Psi(\Phi(\alpha))_{B}(f) = (Ff)(\alpha_{A}(1_{A}))
$$
The [[Naturality Square]] of $\alpha$ at $f$ is:
```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
\mathcal{C}(A,A) \arrow[r,"\mathcal{C}(A{,}f)"] \arrow[d,"\alpha_{A}"]
 & \mathcal{C}(A{,}B) \arrow[d,"\alpha_{B}"] \\
FA \arrow[r,"Ff"]
 & FB
\end{tikzcd}
\end{document}
```
Thus
$$
(Ff)\alpha_{A} = \alpha_{B}( \mathcal{C}(A,f))
$$
where $\mathcal{C}(A,f)$ is actually just $f\cdot$
Thus
$$
\begin{align}
\Psi(\Phi(\alpha))_{B}(f) & = \alpha_{B} (f 1_{A}) = \alpha_{B}(f)  \\
\Psi \Phi(\alpha)  & = \alpha \\
\Psi \Phi  & = 1_{[\mathcal{C},\mathrm{Set}](\mathcal{C}(A,-),F)}
\end{align}
$$
as desired.

Now let us verify that $\Phi$ is a [[Natural Transformation]].
Consider $A\xrightarrow{f}A'$ and $F\xrightarrow{\alpha}F'$ and the diagram:
```tikz
\usepackage{tikz-cd}
\usepackage{amssym}
\begin{document}
\begin{tikzcd}
[\mathcal{C},\mathrm{Set}](\mathcal{C}(A,-),F) \arrow[r,"(f{,}1)"] \arrow[d,"\alpha_{(A{,}F)}"]
 & [\mathcal{C},\mathrm{Set}](\mathcal{C}(A',-),F) \arrow[d,"\alpha_{(A'{,}F)}"] \\
FA \arrow[r,"(Ff{,}1)"]
 & FA'
\end{tikzcd}
\end{document}
```

