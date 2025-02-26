We are given a black box function $f:B_{m}\to B$ which is either constant everywhere (i.e. either 0 or 1 everywhere)
or balanced (i.e. exactly half the inputs give 0)

We want to find whether $f$ is balanced or constant
Classically we need $O(2^{n})$ operations.

Quantum improves:
### The setting
Let $U_{f}\ket{x}\ket{y}=\ket{x}\ket{y\oplus f(x)}$
### The algorithm
#### Step 1
Initialize all qubits in state $\ket{0}$
#### Step 2
$$
(H^{\otimes n}\otimes HX)(\ket{0} ^{\otimes n}\ket{0} )
$$