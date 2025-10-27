[[Category]]
[[Natural Transformation]]
[[Hom-Functor]]
[[Representable]]
[[Representation]]
[[Yoneda Embedding]]
[[Yoneda Lemma]]

[[Product]]
[[Coproduct]]
[[Equalizer]]
[[Coequalizer]]

[[Separating Family]]
[[Detecting Family]]

[[Projective]]
[[Injective]]

[[Adjunction]]
[[Initial]]
[[Terminal]]

[[Comma Category]]
### Corollary
If $F$ and $F'$ are both left [[Adjunction|Adjoint]] to $G:\mathcal{D}\to \mathcal{C}$
then $F$ and $F'$ are [[Isomorphic]] in $[\mathcal{C},\mathcal{D}]$
#### Proof
For any $A$, $(FA,\eta_{A})$ and $(F'A,\eta_{A}')$ are both initial objects of $(A\downarrow G)$
So there's a unique [[Isomorphism]] $\alpha_{A}:(FA,\eta_{A})\to(F'A,\eta_{A}')$
Given $f:A\to A'$, the composits $\alpha_{A'}(Ff)$ and $(F'f)\alpha_{A}$ are both morphisms
$(FA,\eta_{A})\to(F'A',\eta'_{A'}f)$ in $(A\downarrow G)$ so they're equal.
### Lemma
Suppose given $\mathcal{C}\xrightarrow{F}\mathcal{D}\xrightarrow{H}\mathcal{E}$
and $\mathcal{E}\xrightarrow{K}\mathcal{D}\xrightarrow{G}\mathcal{C}$
with $(F\dashv G)$ and $(H\dashv K)$.
Then $(HF\dashv GK)$
#### Proof
We have bijections $\mathcal{C}(A,GKC)\to \mathcal{D}(FA,KC)\to \mathcal{E}(HFA,C)$
which are natural in both $A$ and $C$.
### Corollary
Suppose we are given a [[Commutative Diagram]]
```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
\mathcal{C} \arrow[r,"F"] \arrow[d,"G"]
 & \mathcal{D} \arrow[d,"H"] \\
 \mathcal{E}\arrow[r,"K"]
 & \mathcal{F}
\end{tikzcd}
\end{document}
```
in which all four [[Functor]]s have left [[Adjunction|Adjoint]]s.
Then the square of left adjoints commutes up to [[Natural Isomorphism]].
#### Proof
The two ways round it ar both left [[Adjunction|Adjoint]] to $KG=HF$.
So they must be [[Isomorphic]].

### 
### Proposition
Suppose given an equivalence $\mathcal{C}\xrightarrow{F}\mathcal{D}$ and $\mathcal{D}\xrightarrow{G}\mathcal{C}$
and $\alpha$ and $\beta$ [[Natural Isomorphism]]s
$\alpha:1_{\mathcal{C}}\to GF$ and $\beta:FG\to 1_{\mathcal{D}}$
Then there are [[Natural Isomorphism]]s $\alpha':1_{\mathcal{C}}\to GF$ and $\beta':FG\to 1_{\mathcal{D}}$ 
satisfying the [[Triangular Identities]].
In particular $(F\dashv G)$ and $(G\dashv F)$.
#### Proof
We define $\alpha'=\alpha$ and take $\beta'$ to be 
$$
FG\xrightarrow{(\beta_{FG})^{-1}} 
FGFG\xrightarrow{(F\alpha_{G})^{-1}}
FG\xrightarrow{B}1_{\mathcal{D}}
$$
Note that $FG\beta=\beta_{FG}$ since 
```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
FGFG \arrow[r,"FG\beta"] \arrow[d,"\beta_{FG}"]
 & FG \arrow[d,"\beta"] \\
FG \arrow[r,"\beta"]
 & 1_{\mathcal{D}}
\end{tikzcd}
\end{document}
```
is a [[Commutative Diagram]] by naturality and $\beta$ is [[Monomorphism]].
Similarly $GF\alpha=\alpha_{GF}$
The triangular identities for $\alpha'$ and $\beta'$ are
```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}[column sep=huge]
F \arrow[r,"\alpha_{F}"]
\arrow[dr, swap, "1"]
& GF \arrow[r, "(\beta_{FGF})^{-1}"] 
\arrow[d,"(F_{\alpha})^{-1}"]
& FGFGF \arrow[d,"F_{\alpha_{GF}}"] \\
& F \arrow[r,"(\beta_{F})^{-1}"]
\arrow[dr, swap, "1_{F}"]
& FGF \arrow[d,"\beta_{F}"]
\\
& 
&
F
\end{tikzcd}
\end{document}
```
and 
```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}[column sep=huge]
G \arrow[r,"\alpha_{G}"] 
\arrow[dr,swap,"1_{\mathcal{C}}"]
& GFG \arrow[r,"(GFG\beta)^{-1}"]
\arrow[d,"(\alpha_{G})^{-1}"]
& GFGFG \arrow[d,"(GF\alpha_{G})^{-1}=(\alpha_{GFG})^{-1}"]\\
& G \arrow[r,"(GB)^{-1}"]
\arrow[dr,swap,"1_{G}"]
& GFG \arrow[d,"G\beta"] \\
& & G
\end{tikzcd}
\end{document}
```
so $\alpha'$ and $\beta'$ are the unit and counit of [[Adjunction]] $(F\dashv G)$ 
and $(\beta')^{-1}$ and $(\alpha')^{-1}$ are the unit and counit of $(G\dashv F)$.
