Let $A$ be an [[Object]] of a [[Locally Small]] [[Category]] $\mathcal{C}$ 
and let $F:\mathcal{C}\to \mathrm{Set}$ be a [[Functor]] to [[Category of Sets]]
Then there is a bijection between
[[Natural Transformation]]s $\mathcal{C}(A,\cdot)\to F$ (where $\mathcal{C}(A,\cdot)$ is [[Hom-Functor]])
and elements of $FA$.
Moreover, the bijection is a [[Natural Transformation]] in $A$ and $F$.
### Proof
Given $\alpha:\mathcal{C}(A,\cdot)\to F$ 
Note that $\mathcal{C}(A,A)\xrightarrow{\alpha_{A}}FA$
we define $\Phi(\alpha)=\alpha_{A}(1_{A})\in FA$
Given $x\in FA$ we define $\Psi(x):\mathcal{C}(A,\cdot)\to F$ 
by
$$
\Psi(x)_{B}(A\xrightarrow{f}B) = (Ff)(x)\in FB
$$
Naturality of $\Psi(x)$ follows from [[Functor|functoriality]] of $F$.
We know 
$$
\Phi\Psi(x) = \Psi(x)_{A}(1_{A}) = F(1_{A})(x)=x
$$
And 
$$
\Psi\Phi(\alpha)_{B}(A\xrightarrow{f}B)=(Ff)(\Phi(\alpha))=(Ff)\alpha_{A}(1_{A})=\alpha_{B}(\mathcal{C}(Af)(1_{A}))=\alpha_{B}(f)
$$
for all $B$ and $f$
So $\Phi$ and $\Psi$ are inverse bijections.


