Let $\mathcal H$ be a vector space over $\mathbb C$ (or $\mathbb{R}$) equipped with an [[Inner Product]] $(\cdot, \cdot):\mathcal H \times \mathcal H\to \mathbb C$ (or $\mathbb{R}$)
$\mathcal{H}$ is called a Hilbert space if it is [[Complete]]

[[Closest Point Theorem]]
[[Orthogonal Subspaces]]
### Theorem
If $F$ is a closed subspace of $\mathcal{H}$, then $\mathcal{H}=F\oplus F^{\bot}$.

### Corollary 
1. $F$ is a closed subspace of $\mathcal{H}$ $\implies(F^{\bot})^{\bot}=F$
2. $S\subseteq \mathcal{H}\implies(S^{\bot})^{\bot}=\overline{\langle s \rangle}$
3. $S\subseteq \mathcal{H}$ has dense linear span $\iff S^{\bot}=\{ 0 \}$



## Physical interpretation
Each vector represents a physical space.
Scaling a vector by a complex number represents the same physical state (states correspond to rays in $\mathcal H$) -> useful to work with normalized states
For normalized states, the inner product $(\phi, \psi)$ is the probability amplitude to transition from $\phi$ to $\psi$

We will usually use either a finite dimensional $\mathcal{H}$ (those will usually be our toy models) or an infinite dimensional space of sequences in $\mathbb{C}$ (which converge ie $l_{2}$ ([[L norms]]))