Suppose Alice has a particle in state $\ket{\psi}$ and a particle $A$
Bob also has a particle $B$ and $AB$ is in state $\ket{\phi^{+}}$ [[Bell basis]]
Aim: To send $\ket{\psi}$ to Bob but sending particles is not allowed.

Let $\ket{\psi}=\alpha \ket{0}+\beta \ket{1}$
Initial state has:
$$
\begin{align}
\ket{\psi} _{C}\otimes \ket{\phi^{+}} _{AB} & =(\alpha \ket{0} +\beta \ket{1} )\otimes \frac{1}{\sqrt{ 2 }}(\ket{00} +\ket{11} ) \\
 & =\frac{1}{\sqrt{ 2 }}(\ket{00} +\ket{11} )(\alpha \ket{0} +\beta \ket{1} ) \\
 & +\frac{1}{\sqrt{ 2 }}(\ket{00} -\ket{11} )(\alpha \ket{0} -\beta \ket{1} ) \\
 & +\frac{1}{\sqrt{ 2 }}(\ket{01} +\ket{10} )(\alpha \ket{1} +\beta \ket{0} ) \\
 & +\frac{1}{\sqrt{ 2 }}(\ket{01} -\ket{10} )(\alpha \ket{1} -\beta \ket{0}  \\
 & =\ket{\phi^{+}} \ket{\psi} + \ket{\phi^{-}} (Z\ket{\psi} )+\ket{\psi^{+}} (X\ket{\psi} )+\ket{\psi^{-}} (XZ\ket{\psi} )
\end{align}
$$
Alice does a Bell measurement with outcome $ij$ where $i,j\in \{ 0,1 \}$
She sends $ij$ to Bob.
If $i=0$, $j=1$ what is the post measurement state of $CAB$?
$\ket{\psi^{+}}_{CA}\otimes(X\ket{\psi})_{B}$
Bob's state is $(X\ket{\psi})_{B}$
So Bob should act with $X$ on it to get $X^{2}\ket{\psi}=\ket{\psi}$

In general, if outcome is $ij$ then Bob needs to act on his final state with $Z^{i}X^{j}$ because his final state will be $X^{j}Z^{i}\ket{\psi}$

![[Drawing 2025-02-12 10.31.37.excalidraw]]