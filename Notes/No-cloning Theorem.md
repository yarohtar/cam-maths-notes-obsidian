$CNOT$ can copy a bit value in the first qubit:
$$
CNOT\ket{x} \ket{0} =\ket{x} \ket{x}
$$
when $x\in \{ 0,1 \}$

But can it copy a whole superposition state?
$$
CNOT\ket{\psi} \ket{0} =\ket{\psi} \ket{\psi}
$$
NO!!!
$$
CNOT\ket{\psi} \ket{0} =CNOT(a\ket{0} +b\ket{1} )\ket{0} =a\ket{00} +b\ket{11}
$$
### Theorem
Let $S$ be any set of states of a quantum system, that contains at least one pair of non orthogonal states.
Then there is no unitary cloning process that achieves cloning for all states in $S$.
#### Proof
By contradiction.
Assume there 