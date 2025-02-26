We are given a black box function $f:B_{m}\to B$ which is either constant everywhere (i.e. either 0 or 1 everywhere)
or balanced (i.e. exactly half the inputs give 0)

We want to find whether $f$ is balanced or constant
Classically we need $O(2^{n})$ operations.

Quantum improves:
### The setting
Let $U_{f}\ket{x}\ket{y}=\ket{x}\ket{y\oplus f(x)}$
### The algorithm
#### Step 1
Initialize all qubits in state $\ket{0}^{\otimes n}\ket{0}$
#### Step 2
$$
\begin{align}
(H^{\otimes n}\otimes HX)(\ket{0} ^{\otimes n}\ket{0} )  & = \ket{+} ^{\otimes n}\otimes \ket{-}  \\
 & =\frac{1}{\sqrt{ 2^{n} }}\sum_{x\in B_{n}}\ket{x} \ket{-} \\
 & = \ket{A}  \\
\end{align}
$$
#### Step 4
$$
\begin{align}
U_{f}\ket{A}  & = \frac{1}{\sqrt{ 2^{n} }}\sum_{x\in B_{n}} U_{f}\ket{x} \ket{-}  \\
 & =\frac{1}{\sqrt{ 2^{n} }}\sum_{x\in B_{n}}(U_{f}\ket{x} (\ket{0} -\ket{1} )) \\
 & =\frac{1}{\sqrt{ 2^{n+1} }}\sum_{x\in B_{n}}(\ket{x} \ket{f(x)} -\ket{x} \ket{f(x)^{c}} )
\end{align}
$$
where $\ket{f(x)^{c}}=f(x)\oplus 1$
