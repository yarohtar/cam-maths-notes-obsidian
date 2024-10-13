Let $\{\psi_n\}$ be a complete orthogonal set of wavefunctions, meaning $(\psi_i,\psi_j)=\delta_{ij}$ and any wavefunction $\psi$ can be written as:
$$\psi = \sum_{n=0}^\infty c_n\psi_n$$
Then it follows that $c_n=(\psi,\psi_n)$. More generally, $c_n={(\psi,\psi_n)\over (\psi_n,\psi_n)}$. 

- Any observable $O$ has associated [[Hermetian operator]] $\hat O$.
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

### Commutator
$[\hat A, \hat B] = \hat A\hat B-\hat B\hat A$
Properties:
- $[\hat A, \hat B\hat C] = [\hat A,\hat B]\hat C + \hat B[\hat A,\hat C]$
- $[\hat A\hat B, \hat C] = \hat A[\hat B,\hat C] +[\hat A,\hat C] \hat B$
- $[\hat x, \hat p] = i\hbar$
- $[\hat L_i,\hat L_j]=i\hbar\epsilon_{ijk}\hat L_k$
- $[\hat L^2, \hat L_i]=0$
- $[\hat L_i, \hat H]=0$
- $[\hat L^2,\hat H]=0$