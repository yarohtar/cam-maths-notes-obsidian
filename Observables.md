Observables in Quantum mechanics are represented by [[Linear Operators|linear]] [[Adjoint#Definition|Hermetian]] operators

Operators form an associative but not commutative algebra over $\mathbb{C}$ called the "Operator Algebra" where the product is the composition.
If there is a unique eigenvector for each eigenvalue of an operator $A$, then we label eigenvectors by their eigenvalues and write $A\ket{a}=a\ket{a}$. There is no confusion because the vectors are always in a ket.

If all eigenvectors are nondegenerate we can write
$$
Q=\sum_{n}q_{n}\ket{n} \bra{n}
$$
so that
$$
Q\ket{\psi} =\left( \sum_{n}q_{n}\ket{n} \bra{n}  \right)\left( \sum_{n'}\psi_{n'}\ket{n'}  \right)=\sum_{n}q_{n}\psi_{n}\ket{n} 
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

## Operators for composite systems
Let $\{ \ket{e_{a}} \}$ be basis of $\mathcal{H}_{1}$ and $A:\mathcal{H}\to \mathcal{H}$ a linear operator.
Similarlry $\{ \ket{f_{\alpha}} \}$ and $B$ on $\mathcal{H}_{2}$
We define $A\otimes B:\mathcal{H}_1\otimes \mathcal{H}_{2}\to \mathcal{H}_{1}\otimes \mathcal{H}_{2}$
by
$(A\otimes B)(\ket{e_{a}}\otimes \ket{f_{\alpha}})=(A\ket{e_{a}})\otimes(B\ket{f_{\alpha}})$

Note $[A\otimes \mathbb{1}_{\mathcal{H}_{2}}, \mathbb{1}_{\mathcal{H}_{1}}\otimes B]=0$



