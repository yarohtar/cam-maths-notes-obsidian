Let $\mathcal{C}$ be a [[Small Category]].
The Yoneda embedding is the assignment $A\to \mathcal{C}(A,\cdot)$ and 
$$
\begin{align}
(B\xrightarrow{f}A)
 \longrightarrow 
 \mathcal{C}(f,\cdot): \quad %quad
\mathcal{C}(A,\cdot)  & \to \mathcal{C}(B,\cdot) \\
 (A\xrightarrow{g}C)  & \to (B\xrightarrow{gf}C)
\end{align}
$$
where $\mathcal{C}(A,\cdot)$ is the [[Hom-Functor]].

Alternatively, it is the assignment $B\to \mathcal{C}(\cdot,B)$ and
$$
\begin{align}
(A\xrightarrow{f}B) \longrightarrow \mathcal{C}(\cdot,f): \quad %quad
 \mathcal{C}(\cdot,B)  & \to \mathcal{C}(\cdot,A) \\
(C\xrightarrow{g}B)  & \to (C\xrightarrow{fg}A)
\end{align}
$$
### In words
The Yoneda embedding is a [[Functor]] from $\mathcal{C}^{op}$ to $[\mathcal{C},\mathrm{Set}]$ (see [[#Lemma]])
sending each object $A\in \operatorname{ob}\mathcal{C}$ to a [[Hom-Functor]] $\mathcal{C}(A,\cdot)$
and sending each [[Morphism]] $B\xrightarrow{f}A$
to a [[Natural Transformation]] $\mathcal{C}(A,\cdot)\to \mathcal{C}(B,\cdot)$.
In particular, this [[Natural Transformation]] corresponding to $B\xrightarrow{f}A$
assigns to each [[Object]] $C\in \operatorname{ob}\mathcal{C}$
a [[Morphism]] between [[Hom-Set]]s $\mathcal{C}(A,C)\to \mathcal{C}(B,C)$ 
[[Morphism]]s in the [[Category of Sets]] are just functions between them,
so in particular, for any $g\in \mathcal{C}(A,C)$ we assign it a $gf\in \mathcal{C}(B,C)$
### Lemma
The Yoneda embedding defines a [[Full]] and [[Faithfull]] [[Functor]] $\mathcal{C}^{op}\to[\mathcal{C},\mathrm{Set}]$
### Proof
Putting $F=\mathcal{C}(B,\cdot)$ in [[Yoneda Lemma]], 
we find that the Yoneda Embedding is a bijection from $\mathcal{C}(B,A)$ 
to the collection of [[Natural Transformation]]s $\mathcal{C}(A,\cdot)\to \mathcal{C}(B,\cdot)$
Thus this will automatically be [[Full]] and [[Faithfull]].
The [[Functor|functoriality]] of this follows from [[Associativity]] of composition in $\mathcal{C}$

