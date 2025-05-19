Let $n$ be odd.
Let $K$ be a field extension of $\mathbb{F}_{2}$ containing all $n^{th}$ roots 
of unity $\{ 1, \alpha, \alpha^{2},\dots,\alpha^{n-1} \}$ (e.g. $K=\mathbb{F}_{2^{r}}$ for $2^{r}=1\pmod{n}$)
A BCH code with design distance $\delta$
is a [[Cyclic Code with Defining Set]] $A=\{ \alpha,\alpha^{2},\dots,\alpha^{\delta-1} \}$
### Lemma
The generator $g(X)$ for BCH code $C$ is 
$$
\operatorname{lcm} \{ m_{1}(X), \dots, m_{\delta-1}(X) \}
$$
where $m_{i}(X)$ is the minimal polynomial for $\alpha^{i}$ over $\mathbb{F}_{2}$
### Theorem
The [[Minimum distance of a code]] for BCH code is at least the design distance $\delta$.
#### Proof
Consider the matrix:
$$
H=\begin{pmatrix}
1 & \alpha & \alpha^{2} & \dots & \alpha^{n-1} \\
1 & \alpha^{2} & \alpha^{4} & \dots & \alpha^{2(n-1)} \\
\vdots & \vdots & \vdots & \ddots & \vdots \\
1 & \alpha^{\delta-1} & \alpha^{2(\delta-1)} & \dots & \alpha^{(\delta-1)(n-1)}
\end{pmatrix}
$$
Taking any $\delta-1$ columns, gives a [[Vandermonde matrix]], 
so any $\delta-1$ columns of $H$ are linearly independent.
But a codeword in $C$ is a dependence relation 
between the columns of $H$ so $w(C)\geq\delta$

Note that $H$ is not the [[Parity Check Matrix]] 
in the usual sense, because $\alpha \not\in \mathbb{F}_{2}$
# Decoding
Suppose we receive $r=c+e$ where $e$ is the error pattern
### Definition
The error locator polynomial of an error pattern $e\in \mathbb{F}_{2}^{n}$ is
$$
\sigma(X)=\prod_{i\in \mathcal{E}}(1-\alpha^{i}X)\in K[X]
$$
where $\mathcal{E}=\{ i: e_{i}=1 \}$.
Note that $\sigma(\alpha^{n-i})=0$, so if we know $\sigma$ we can recover all errors
### Theorem
Suppose $\operatorname{deg}\sigma=\lvert \mathcal{E} \rvert\leq t$ where $2t+1\leq\delta$.
$\sigma(X)$ has constant term 1 and satisfies:
$$
\sigma(X)\sum_{j=1}^{2t} r(\alpha^{j})X^{j}
$$
#### Proof