### Helstrom and Hovelo Theorem
You are given a quantum system in unknown state $\ket{\psi}$
You are told $\ket{\psi}$ is either in $\ket{\alpha_{0}}$ or $\ket{\alpha_{1}}$ with probability $\frac{1}{2}$
Do a 2-outcome measurement
Probability of success

$$
\begin{align}
p\left(\Pi_{0} \right) & =\frac{1}{2}+\frac{1}{2}Tr(\Pi_{0}(\ket{\alpha_{0}} \bra{\alpha_{0}} -\ket{\alpha_{1}} \bra{\alpha_{1}} )) \\
 & =\frac{1}{2}+\frac{1}{2}Tr(\Pi_{0}\Delta)
\end{align}
$$
Properties 
$\Delta ^{\dagger}=\Delta$
$\ket{\beta}\in \mathcal{H}$ s.t. $\braket{ \beta | \alpha_{0} }=0=\braket{ \beta | \alpha_{1} }$
then $\Delta \ket{\beta}=0$
$Tr\Delta=0$ so eigenvalues are $+\delta$ and $-\delta$
Let corresponding eigenvalues be $\ket{p},\ket{m}$ and $P_{\delta}=\ket{p}\bra{p}$ and $P_{-\delta}=\ket{m}\bra{m}$
Spectral decomposition: $\Delta=\delta P_{\delta}-\delta P_{-\delta}$
Determine $\delta$ in terms of $\ket{\alpha_{0}}$, $\ket{\alpha_{1}}$
Let $\ket{\alpha_{0}^{\bot}}$