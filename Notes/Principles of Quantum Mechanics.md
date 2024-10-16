(caution: my notes on PQM could have cursed bits for somebody who actually knows physics)

Notes by David Skinner
https://www.damtp.cam.ac.uk/user/dbs26/PQM.html

[[Hilbert Spaces (PQM)]]
[[Dual Spaces (PQM)]]
[[Dirac Notation]]
[[Continuum States]]
[[Different basis (PQM)]]
[[Tensor Product of Hilbert Spaces]]

[[Postulates of QM]]
[[Commutator]]
[[Adjoint]]

If all eigenvectors are nondegenerate we can write
$$
Q=\sum_{n}q_{n}\ket{n} \bra{n}
$$
so that
$$
Q\ket{\psi} =\left( \sum_{n}q_{n}\ket{n} \bra{n}  \right)\left( \sum_{n'}\psi_{n'}\ket{tn'}  \right)=\sum_{n}q_{n}\psi_{n}\ket{n} 
$$
Define $f(Q)=\sum_{n}f(q_{n})\ket{n}\bra{n}$ defines $f(Q)$ if $f(\phi_{n})$ exists.

Matrix elements of $A$ in this basis are $A_{nn'}=\bra{n}A\ket{n'}$.

Also $(AB)_{nn'}=\bra{n}AB\ket{n'}=\sum_{k}A_{nk}B_{kn'}$
Also $(A^{\dagger})_{nn'}=(A_{n'n})^{*}$


When e-vectors of $Q$ are degenerate, we look for a complete set of commuting observables $\{ Q, P, \dots \}$ st $[Q,P]=0=[\dots]$ for all pairs.

Then they are simultaneously diagonalizable (diagonalizable in the same basis)
$\{ \ket{q_{m},p_{m},\dots }\}$

### Operators in $dim\mathcal{H}=\infty$
Let's menttion and ignore some issues in spaces such as $L^2(\mathbb{R},dx)$
[[Linear Operators#Definition]] (bounded operators)
- In finite dim all operators are bounded
- In infinite dimensions thats not true. Position and momentum operators are unbounded
