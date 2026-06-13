Let $\mathcal{L}$ be a [[Language]].
Let $T$ be a [[Consistent]] $\mathcal{L}$-[[Theory]] 
Define the equivalence relation on formulas 
$\varphi \sim \psi$ if and only if $T\vdash (\varphi \iff \psi)$,
and for each $n\in \mathbb{N}$ fix variables $x_{1},x_{2},\dots,x_{n}$ let 
$$
F_{n}=\{ [\varphi]: \text{$\varphi$ has free variables $x_{1},\dots,x_{n}$}\}
$$
Clearly $F_{n}$ is a [[Boolean Algebra]].
The $n$-type space over $T$ is defined as the [[Stone Space]] of $F_{n}$
and we write 
$$
S_{n}(T) = S(F_{n})
$$
The elements of this space are $n$-[[Formula Type]]s.

Moreover, if $\mathcal{M}$ is an $\mathcal{L}$-[[Structure]] and $A\subseteq M$ we define 
$$
S_{n}^{\mathcal{M}}(A)=S_{n}(\mathrm{Th}_{A}(\mathcal{M}))
$$
where $\mathrm{Th}_{A}(\mathcal{M})$ are all theorems of $\mathcal{M}$ when seen as an $\mathcal{L}_{A}$-[[Structure]] 
for $\mathcal{L}_{A}$ the language $\mathcal{L}$ extended by constant symbols $\{ t_{a} : a\in A \}$
and $t_{a}^{\mathcal{M}}=a$.

Note that this is always defined as $\mathrm{Th}_{A}(\mathcal{M})$ is [[Consistent]]
as it has a model $\mathcal{M}$.
### Lemma
Formula type space is [[Compact]] [[Hausdorff]] [[Totally Disconnected]].
#### Proof
Follows from [[Stone Space]].
### Proposition


