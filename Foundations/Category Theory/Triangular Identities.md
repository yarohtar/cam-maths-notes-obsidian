Given [[Functor]]s $\mathcal{C}\xrightarrow{F}\mathcal{D}$ and $\mathcal{D}\xrightarrow{G}\mathcal{C}$,
specifying an adjunction $(F\dashv G)$
is equivalent to specifying [[Natural Transformation]]s 
$\eta:1_{\mathcal{C}}\to GF$ and $\varepsilon:FG\to 1_{\mathcal{D}}$ satisfying
```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
F \arrow[r,"F\eta"] 
\arrow[dr,swap, "1_{F}"] 
& FGF \arrow[d,"\varepsilon_{F}"] \\
& F
\end{tikzcd}
\end{document}
```
```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
G \arrow[r,"1_{G}"] 
\arrow[dr,swap, "1_{\mathcal{C}}"] 
& GFG \arrow[d,"G\varepsilon"] \\
& G
\end{tikzcd}
\end{document}
```
the triangular identities.
#### Proof
Given $(F\dashv G)$, let $\eta$ and $\varepsilon$ be [[Unit]] and [[Counit]] respectively.
Then $\varepsilon_{FA}(F\eta_{A})$ corresponds under the [[Adjunction]] to $1_{GFA}\eta_{A}=\eta_{A}$, so it's $1_{FA}$. 
The second identity is dual.
Conversely, suppose given $\eta$ and $\varepsilon$ satisfying triangular identities.
Given $A\xrightarrow{f}GB$ we define $\Phi(f)$ to be $FA\xrightarrow{Ff}FGB\xrightarrow{\varepsilon_{B}}B$
and given $FA\xrightarrow{g}B$ we define $\Psi(g)$ to be $A\xrightarrow{\eta_{A}}GFA\xrightarrow{Gg}GB$
Then $\Psi \Phi(f)$ is 
```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
A\arrow[r,"\eta_{A}"] 
\arrow[dr, "f"] 
& GFA \arrow[r,"GFf"]
& GFGB \arrow[r,"G\varepsilon_{B}"]
& GB \\
& GB \arrow[ru, "\eta_{GB}"]
\arrow[rru,swap, "1_{GB}"]
\end{tikzcd}
\end{document}
```
so $\Psi \Phi(f)=f$ and dually $\Phi \Psi(g)=g$ 
And $\Phi$ and $\Psi$ are natural since $\eta$ and $\varepsilon$ are.