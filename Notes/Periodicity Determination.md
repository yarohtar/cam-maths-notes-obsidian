### Input
Black box for a function $f:\mathbb{Z}_{N}\to \mathbb{Z}_{M}$
$f$ is periodic with a period $r$ 
### Output
Return $r$ with some desired accuracy independent of $N$ 

### Algorithm
Construct
$$
\ket{\psi_{N}} =\frac{1}{\sqrt{ N }}\sum_{x\in \mathbb{Z}_{N}}\ket{x} 
$$
Consider a state $\ket{\psi_{N}}.\ket{0}$ (where $\ket{0}\in \mathcal{H}_{N}$)
Apply the quantum oracle of the function $f$ 
$$
\begin{align}
U_{f}\ket{\psi_{N}} \ket{0}  & =\frac{1}{\sqrt{ N }}\sum_{x\in \mathbb{Z}_{N}}U_{f}\ket{x} \ket{0}  \\
 & =\frac{1}{\sqrt{ N }}\sum \ket{x} \ket{0+f(x)}  \\
 & =\frac{1}{\sqrt{ N }}\sum_{x\in \mathbb{Z}_{N}}\ket{x} \ket{f(x)} 
\end{align}
$$
Since $r$ is the period of $f$:
$r\mid N$ and let $A=\frac{N}{r}$ be the number of periods

Do a measurement on the second register of basis $\mathcal{B}_{M}=\{ \ket{0,\dots,\ket{M-1}} \}$
Let outcome be $y=f(x_{0})$
$x_{0}\in \{ 0,1,\dots,r-1 \}$ is the smallest value of $x$ for which $f(x)=y$

