# General definition
Let $\mathcal{H}$ be a [[Hilbert Space]]. 
Consider a collection of operators $\{ \mathcal{M}_{n} \}_{n} \subseteq \mathcal{B(\mathcal{H})}$ with $\sum_{n}M_{n}^{*}M_{n}=\mathbb{1}$
Suppose we have a state $\ket{\phi}$
$$
\left\{ \ket{n}  \text{ with prob } p(n)=\braket{ \phi | M_{n}^{*}M_{n}\phi }   \right\}\to^\text{mmt} \frac{M_{n}\ket{\phi} }{\sqrt{ p(n) }}
$$

## Projective measurement
## Positive operator valued measurement (POVM)
$E_{n}=M_{n}^{*}M_{n}$ [[Positive semi-definite]]
$M_{n}=\sqrt{ E_{n} }$
## Unitary Evolutions

# Part IB/II
Let $\{\psi_n\}$ be a complete orthogonal set of wavefunctions, meaning $(\psi_i,\psi_j)=\delta_{ij}$ and any wavefunction $\psi$ can be written as:
$$\psi = \sum_{n=0}^\infty c_n\psi_n$$
Then it follows that $c_n=(\psi,\psi_n)$. More generally, $c_n={(\psi,\psi_n)\over (\psi_n,\psi_n)}$. 

- Any observable $O$ has associated [[Adjoint|Hermetian operatorr]] $\hat O$.
- Hence, for any observable, we can write $\psi$ as a linear combination of eigenfunctions of $\hat O$.
- The outcome of a measurement is always an eigenvalue of $\hat O$.
- After a measurement with outcome $\lambda$, the wavefunction collapses to a linear combination of eigenfunctions with eigenvalue $\lambda$
- The probability of an outcome $\lambda_n$ is $|c_n|^2$ (or the sum of appropriate stuff)
- The expected value of $O$ is $\langle\hat O \rangle_\psi = \int\psi^*\hat O\psi dV$

## Examples
- Position operator is $\hat x=x$
- Momentum operator is $\hat p =-i\hbar {\partial\over \partial x}$
- Energy operator is $\hat H= {\hat p^2\over 2m} +V(\hat x)$
- Angular momentum operator is $\hat L=\hat x\times\hat p=-i\hbar\hat x\times\nabla$ 


[[Commutator]]

### Composite system
Suppose we have $\mathcal{H}=\mathcal{H}_{1}\otimes \mathcal{H}_{2}$ with basis $\mathcal{B}=\{ \ket{e_{i}}\otimes \ket{f_{j}} \}$
and we want to only measure in the basis $\{ \ket{e_{i}} \}$
We take $\mathcal{H}=\oplus_{i=1}^{m}\mathcal{E}_{i}$
where
$$
\mathcal{E}_{i}=span\{ \ket{e_{i}} \otimes \ket{\phi} : \ket{\phi} \in \mathcal{H}_{2} \}
$$
and take the projective measurements in these subspaces and etc whatever ... 
