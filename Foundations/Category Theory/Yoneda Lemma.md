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
Given $\alpha:\mathcal{C}(A,-)\to F$ a [[Natural Transformation]]
Note that $\mathcal{C}(A,A)\xrightarrow{\alpha_{A}}FA$
so define $\Phi(\alpha)=\alpha_{A}(1_{A})\in FA$
Given $x\in FA$ 
we define a [[Natural Transformation]] $\Psi(x):\mathcal{C}(A,-)\to F$ by
$$
\begin{align}
\Psi(x)_{B} : \mathcal{C}(A,B) & \to FB \\
(A\xrightarrow{f}B)  & \to(Ff)(x)
\end{align}
$$
To get naturality of $\Psi$ we need to show for any $f:B\to C$
$$
\Psi_{B}(x)\mathcal{C}(A,f) = (Ff) \Psi_{A}(x)
$$
i.e. for any $g\in \mathcal{C}(A,B)$:
$$
(F(gf))(x) = (Ff)(Fg)(x)
$$
which is follows from [[Functor|functoriality]] of $F$.
We know 
$$
\Phi\Psi(x) = \Psi(x)_{A}(1_{A}) = F(1_{A})(x)=x
$$
And for all $B$ and $f$ we have a [[Commutative Diagram]]:
```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
\mathcal{C}(A,A) \arrow[r,"\mathcal{C}(A{,}f)"] \arrow[d,"\alpha_{A}"]
 & \mathcal{C}(A,B) \arrow[d,"\alpha_{B}"] \\
FA \arrow[r,"Ff"]
 & FB
\end{tikzcd}
\end{document}
```
so we can calculate:
$$
\Psi(\Phi(\alpha))_{B}(A\xrightarrow{f}B)=(Ff)(\Phi(\alpha))=(Ff)\alpha_{A}(1_{A})=\alpha_{B}\mathcal{C}(A,f)(1_{A})=\alpha_{B}(f)
$$
i.e. 
$$
\Psi(\Phi(\alpha))=\alpha
$$
So $\Phi$ and $\Psi$ are inverse bijections.


