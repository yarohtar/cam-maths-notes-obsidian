We say a [[Functor]] $F:\mathcal{C}\to \mathrm{Set}$ is representable 
if it's [[Isomorphic]] to the [[Hom-Functor]] $\mathcal{C}(A,-)$ for some $A$,
i.e. there is some [[Natural Isomorphism]] $\mathcal{C}(A,-)\to F$

We also say a [[Contravariant]] [[Functor]] $F:\mathcal{C}\to \mathrm{Set}$ is representable 
if it's [[Isomorphic]] to the the [[Contravariant]] [[Hom-Functor]] $\mathcal{C}(-,A)$ for some $A$.

### Example
The identity functor $1_{\mathrm{Set}}:\mathrm{Set}\to \mathrm{Set}$ is representable.
In particular, take the functor $\mathrm{Set}(1,-)$.
For any set $B$, we have $\mathrm{Set}(1,B)$ [[Isomorphic]] to $B$
The [[Natural Isomorphism]] is defined by sending $B$ 
to a function $\alpha_{B}:\mathrm{Set}(1,B)\to B$ 
sending 
$$
\alpha_{B}(1\xrightarrow{f}B) = f(0)
$$
(where $0\in 1$ is the only element of $1$).
This is clearly invertible.
### Example
The [[Forgetful Functor]] $U:\mathrm{Gp}\to \mathrm{Set}$ is representable.
In particular consider $\mathrm{Gp}(\mathbb{Z},-)$.
For a [[Group]] $G$ we can find $\alpha_{G}:\mathrm{Gp}(\mathbb{Z},G)\to U(G)$
defined by:
$$
\alpha_{G}(\mathbb{Z}\xrightarrow{f} G) = (Uf)(1)
$$
Note that we needed to "forget" that $f$ is a [[Homomorphism]],
in order to be able to use it as a normal function between sets $U(\mathbb{Z})$ and $U(G)$.
We can then check that $\alpha$ is a [[Natural Isomorphism]]


with [[Representation]] $(\mathbb{Z},1)$.
That is, for any [[Group]]s $G,H\in \operatorname{ob}\mathrm{Gp}$
with a [[Homomorphism]] $f:G\to H$ 
we can have a [[Natural Isomorphism]] $\alpha$
and a [[Commutative Diagram]]
```tikz
\usepackage{tikz-cd}
\usepackage{amssymb}
\begin{document}
\begin{tikzcd}
\mathcal{C}(\mathbb{Z},G) \arrow[r,"\mathcal{C}(\mathbb{Z}{,}f)"] \arrow[d,"\alpha_{G}"]
 & \mathcal{C}(\mathbb{Z},H) \arrow[d,"\alpha_{H}"] \\
FG \arrow[r,"Ff"]
 & FH
\end{tikzcd}
\end{document}
```
where $\alpha_{G}$ sends a [[Homomorphism]] $g:\mathbb{Z}\to G$
to the element $g(1)$



