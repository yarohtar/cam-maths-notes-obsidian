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
