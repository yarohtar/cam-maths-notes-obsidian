Let $\mathcal{A}:\mathcal{B}\to \mathcal{B}_{R}$ be a [[Combinatorial Structure]].
For each $S\in \mathcal{B}$ define an equivalence relation $\sim$ on $\mathcal{A}(S)$ by:
$$
a\sim b \iff \mathcal{A}(\sigma)(a) = b
$$
for some bijective $\sigma:S\to S$.
The unlabelled structure from $\mathcal{A}$ is the set of equivalence classes of $\sim$.
We write $\mathcal{A}_{n}=\mathcal{A}[n]/\sim$ for equivalence classes of $\mathcal{A}$-structures of order $n$.

Note that the weight $w:\mathcal{A}(S)\to R$ satisfies
$$
a\sim b \implies w(a) = w(b)
$$
so we can define $w([a])=w(a)$
as the weight on the equivalence classes of $\sim$.

Each unlabelled structure has an associated [[Ordinary Generating Function]]

