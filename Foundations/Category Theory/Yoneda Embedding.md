Let $\mathcal{C}$ be a [[Small Category]].
The Yoneda embedding is the assignment $A\to \mathcal{C}(A,\cdot)$
where $\mathcal{C}(A,\cdot)$ is the [[Hom-Functor]].

### Lemma
The mapping $A\to \mathcal{C}(A,\cdot)$ defines a [[Full]] and [[Faithfull]] [[Functor]] $\mathcal{C}^{op}\to[\mathcal{C},\mathrm{Set}]$
### Proof
Putting $F=\mathcal{C}(B,\cdot)$ in [[Yoneda Lemma]], 
we get a bijection from $\mathcal{C}(B,A)$ to the collection of
[[Natural Transformation]]s $\mathcal{C}(A,\cdot)\to \mathcal{C}(B,\cdot)$
This sends $f\in \mathcal{C}(B,A)$ to $\Psi(f):\mathcal{C}(A,\cdot)\to \mathcal{C}(B,\cdot)$
such that any $A\xrightarrow{g}B$ is sent to $gf$.
which is given by composition by $f$ 
So [[Functor|functoriality]] follows from [[Associativity]] of composition in $\mathcal{C}$
Dually, we have a [[Full]] and [[Faithfull]] [[Functor]] $\mathcal{C}\to[\mathcal{C}^{op},\mathrm{Set}]$ sending $B$ to $\mathcal{C}(\cdot,B)$

