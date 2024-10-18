The Hamiltonian in 1d is
$$
H=\frac{p^{2}}{2m}+\frac{m\omega^{2}}{2}X^{2}
$$
Introduce dimensionless lowering and raising operators
$$
\begin{gather}
A=\frac{1}{\sqrt{ 2m\omega \hbar }}(m\omega X+iP)\\
A^{\dagger}=\frac{1}{\sqrt{ 2m\omega \hbar }}(m\omega X-iP)
\end{gather}
$$
Since 
$$
\begin{align}
A^{\dagger}A & =\frac{1}{2m\omega \hbar}(m\omega X-iP)(m\omega X+iP) \\
 & =\frac{1}{2m\omega \hbar}(P^{2}+m^{2}\omega^{2}X^{2}+im\omega[X,P]) \\
 & =\frac{H}{\hbar \omega}-\frac{1}{2}
\end{align}
$$
the Hamiltonian becomes 
$$
H=\hbar \omega\left( A^{\dagger}A+\frac{1}{2} \right)
$$
Call $N=A^{\dagger}A$ the ([[Hermetian operator|Hermetian]]) number operator.
We now have operators but we don't have the [[Hilbert Spaces (PQM)|Hilbert space]].
Start from the operator algebra $\{ X^nP^m \}$ and commutation relation $[X,P]=i\hbar$. $\mathrm{Im}$ terms of $A^{\dagger},A$:
$$
[A,A^{\dagger}]=\frac{1}{2m\omega \hbar}[m\omega X+iP,m\omega X-iP]=-\frac{im\omega e}{2m\hbar \omega}([X,P]-)
$$