---
aliases:
  - Adjoint
---
Let $\mathcal{C}$ and $\mathcal{D}$ be [[Category|Categories]]
Let $F:\mathcal{C}\to \mathcal{D}$ and $G:\mathcal{D}\to \mathcal{C}$ be [[Functor]]s
We say that $F$ is left adjoint to $G$ and $G$ is right adjoint to $F$ if
$$
\mathcal{C}(A,GB) \cong \mathcal{D}(FA,B)
$$
naturally in $A\in \mathcal{C}$ and $B\in \mathcal{D}$. We write $F\dashv G$
An adjunction between $F$ and $G$ is this [[Isomorphism]].

### what does naturally mean?
If $\mathcal{C}$ and $\mathcal{D}$ were [[Locally Small]], we could express it as a [[Natural Isomorphism]] 
$$
\mathcal{C}(-,G-) \to \mathcal{D}(F-,-)
$$
as functors $\mathcal{C}^{op}\times \mathcal{D}\to \mathrm{Set}$.
If they are not locally small we can express this in elementary terms as follows.
For $f:A\to GB$ in $\mathcal{C}$ denote by $\overline{f}:FA\to B$ the corresponding [[Morphism]] in $\mathcal{D}$
Similarly, for any $g:FA\to B$ denote by $\overline{g}:A\to GB$...

Naturality means that for any $q:B\to B'$ and $p:A'\to A$ we have
$$
\overline{qg(Fp)}=(Gq)\overline{g}p
$$
or equivalently 
$$
\overline{(Gq)fp} = q \overline{f} (Fp)
$$
Note that I actually couldn't write anything else sensible with these symbols.
This is because its the only "natural" thing to write down.

## Theorem
Let $G:\mathcal{D}\to \mathcal{C}$ be a [[Functor]].
Then specifying a left [[Adjunction|Adjoint]] for $G$
is equivalent to
specifying an [[Initial]] object of the [[Comma Category]] $(A\downarrow G)$ 
for each $A\in \operatorname{ob}\mathcal{C}$.
### Proof
#### $\implies$
Suppose $G$ has a left [[Adjunction|Adjoint]] $F:\mathcal{C}\to \mathcal{D}$.
Let $\eta_{A}:A\to GFA$ be the morphism corresponding to $1_{FA}$ 
Then $(FA, \eta_{A})$ is [[Initial]] in $(A\downarrow G)$. 
Let $(B,f)$ be an object in $(A\downarrow G)$ where $f:A\to GB$
A map $q:(FA,\eta_{A})\to(B,f)$ in $(A\downarrow G)$ is $q:FA\to B$ in $\mathcal{D}$
such that we have a [[Commutative Diagram]]
```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
A \arrow[r, "\eta_{A}"] \arrow[dr,swap, "f"] 
& GFA \arrow[d, "Gq"] \\
& GB
\end{tikzcd}
\end{document}
```
i.e.
$$
f=(Gq)\eta_{A}
$$
But these correspond uniquely to
$$
\overline{f}=q \overline{\eta_{A}} = q 1_{FA} = q
$$
Thus $q=\overline{f}$ exists and is unique.
#### $\impliedby$
Suppose for any $A$ we are given an initial object $(FA,\eta_{A})$ of $(A\downarrow G)$
This defines a [[Functor]] $F$ on objects $A\in \mathcal{C}$.
For any $f:A\to B$ define $Ff$ to be the unique $(FA,\eta_{A})\to(FB,\eta_{B})$ in $(A\downarrow G)$
Then $Ff$ is a morphism $FA\to FB$ 
and [[Functor|functoriality]] of $F$ follows from uniqueness.
The [[Adjunction]] sends each $f:A\to GB$
to the unique $(FA,\eta_{A})\to(B,f)$ in $(A\downarrow G)$.
On the other hand, each $g:FA\to B$ 
is sent to $(Gg)\eta_{A}$ and we can verify naturality.