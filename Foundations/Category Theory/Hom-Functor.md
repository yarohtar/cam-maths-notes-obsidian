Let $\mathcal{C}$ be [[Locally Small]].
We define the [[Covariant]] hom-functor to be:
$$
\mathcal{C}(A,-):\mathcal{C}\to \mathrm{Set}
$$
We send each object $B\in\operatorname{ob}\mathcal{C}$ to the [[Hom-Set]] $\mathcal{C}(A,B)$
We send each morphism $g:B\to C$ to a function
$$
\mathcal{C}(A,g):\mathcal{C}(A,B) \to \mathcal{C}(A,C)
$$
defined by 
$$
\mathcal{C}(A,g)(h)=gh
$$

Similarly, the [[Contravariant]] hom-functor 
$$
\mathcal{C}(-,B):\mathcal{C}\to \mathrm{Set}
$$
sends $A$ to $\mathcal{C}(A,B)$ 
and $g:C\to A$ to the map $\mathcal{C}(g,B):\mathcal{C}(A,B)\to \mathcal{C}(C,B)$
given by
$$
\mathcal{C}(g,B)(h) = hg
$$
### Lemma
The [[Covariant]] hom-functor $\mathcal{C}(A,-)$ is a [[Functor]].
Similarly, the [[Contravariant]] hom-functor $\mathcal{C}(-,B)$ is a [[Contravariant]] [[Functor]].
### Proof
[[Functor]]iality follows from the [[Associativity]] law in $\mathcal{C}$

## what does this really say?
The covariant hom-functor $\mathcal{C}(A,-)$ is telling us how $A$ sees the [[Category]] $\mathcal{C}$
The contravariant hom-functor $\mathcal{C}(-,A)$ is telling us how $A$ is seen by $\mathcal{C}$.
