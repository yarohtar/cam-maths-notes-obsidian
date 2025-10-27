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

