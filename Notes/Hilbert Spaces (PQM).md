### Definition
Hilbert space $\mathcal H$ is a vector space over $\mathbb C$ equipped with an inner product $(\cdot, \cdot):\mathcal H \times \mathcal H\to \mathbb C$ where
1. $(\phi,\psi)=(\psi,\phi)^*$
2. $(\phi, a\psi)=a(\phi,\psi)$ but $(a\phi, \psi)=a^*(\phi,\psi)$
3. $(\phi,\phi)\geq 0$ with equality iff $\phi=0$
This inner product defines a [[Normed Spaces|norm]] $||\psi||=\sqrt{(\psi,\psi)}$.

$\mathcal H$ is complete with this norm: a Cauchy sequence converges in $\mathcal H$. Can take limits and derivatives.

## Physical interpretation
Each vector represents a physical space.
Scaling a vector by a complex number represents the same physical state (states correspond to rays in $\mathcal H$) -> useful to work with normalized states
For normalized states, the inner product $(\phi, \psi)$ is the probability amplitude to transition from $\phi$ to $\psi$

We will usually use either a finite dimensional $\mathcal{H}$ or a countably dimensional space of sequences in $\mathbb{C}$.