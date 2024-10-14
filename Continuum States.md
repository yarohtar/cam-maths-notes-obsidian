Usually we expand in ccountable orthonormal basis $\ket{\psi}=\sum_{m}a_{m}\ket{\psi_{m}}$ and $\braket{ \phi_{n} | \phi_{m} } =\delta_{nm}$

Sometimes we generalize this to continuum states

Consider $L^2(\mathbb{R},dx)$
For $x\in \mathbb{R}$ let $\ket{x}$
define operator $X\ket{x}=x\ket{x}$ and $\braket{ x' | x }=\delta(x-x')$
Then we can expand any vector as
$$
\ket{\psi} = \int_{\mathbb{R}}\psi(x')\ket{x'} dx'
$$
We extract the wavefunction by projecting on $\ket{x}$
$$
\braket{ x | \psi } =\int \psi(x')\braket{ x | x' } dx'=\int \psi(x')\delta(x-x')dx'=\psi(x)
$$
