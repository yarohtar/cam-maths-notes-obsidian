Let $\mathcal{C}$ be a [[Small Category]].
The collection of [[Hom-Functor]]s $\mathcal{C}(A,-)$ when $A\in \operatorname{ob}\mathcal{C}$
gives us a way to see $\mathcal{C}$ from the perspective of each object $A$.
It is always the same [[Category]] that's being seen, 
so there must be something nice that these [[Hom-Functor]]s satisfy.

In particular, each [[Morphism]] $A\xrightarrow{f}B$ in $\mathcal{C}$ induces a [[Natural Transformation]]
$$
\mathcal{C}(f,-): \mathcal{C}(B,-)\to \mathcal{C}(A,-)
$$
given by $\mathcal{C}(f,-)_{C}=\mathcal{C}(f,C)$ 
i.e. the [[Contravariant]] [[Hom-Functor]] $\mathcal{C}(-,C)$ evaluated at $f$.

Moreover, for any $A\xrightarrow{f}B\xrightarrow{g}C$ we have
$$
\mathcal{C}(fg,-) = \mathcal{C}(f,-) \mathcal{C}(g,-)
$$
because 

The Yoneda embedding of $\mathcal{C}$ is the [[Contravariant]] [[Functor]]
$$
\mathcal{C}(\bullet,-): \mathcal{C} \to [\mathcal{C},\mathrm{Set}]
$$
sending objects $A\in \operatorname{ob}\mathcal{C}$ to [[Hom-Functor]]s $\mathcal{C}(A,-)$, 
and sending [[Morphism]]s $A\xrightarrow{f}B$ to [[Natural Transformation]]s 
$$
\mathcal{C}(f,-):\mathcal{C}(B,-)\to \mathcal{C}(A,-)
$$
defined by:
$$
\mathcal{C}(f,-)_{C} = \mathcal{C}(f,C) : \mathcal{C}(B,C) \to \mathcal{C}(A,C) 
$$
given by
$$
\mathcal{C}(f,C)(g) = gf
$$

Alternatively, the Yoneda embedding is the [[Covariant]] [[Functor]]
$$
\mathcal{C}(-,\bullet): \mathcal{C} \to [\mathcal{C},\mathrm{Set}]
$$
sending objects $A\in \operatorname{ob}\mathcal{C}$ to [[Hom-Functor]]s $\mathcal{C}(-,A)$
and sending [[Morphism]]s $A\xrightarrow{f}B$ to [[Natural Transformation]]s
$$
\mathcal{C}(-,f): \mathcal{C}(-,A) \to \mathcal{C}(-,B)
$$
defined by:
$$
\mathcal{C}(-,f)_{C} = \mathcal{C}(C,f) : \mathcal{C}(C,A) \to \mathcal{C}(C,B)
$$
given by:
$$
\mathcal{C}(C,f)(g) = fg
$$
### Lemma
Yoneda embedding is a [[Functor]].
#### Proof
Follows from [[Associativity]] of composition in $\mathcal{C}$.
### Lemma
The Yoneda embedding defines a [[Full]] and [[Faithfull]] [[Functor]] $\mathcal{C}^{op}\to[\mathcal{C},\mathrm{Set}]$
### Proof
Putting $F=\mathcal{C}(B,-)$ in [[Yoneda Lemma]], 
we find that the Yoneda embedding is a bijection from $\mathcal{C}(B,A)$ 
to the collection of [[Natural Transformation]]s $\mathcal{C}(A,-)\to \mathcal{C}(B,-)$
Thus this will automatically be [[Full]] and [[Faithfull]].

