The dual of $X$ is $X^{*}=L(X,\mathbb{R})$ the set of all linear functionals from $X$ to $\mathbb{R}$.

### Definition
For normed spaces $X$ and $Y$, an isomorphism from $X$ to $Y$ is a map $T:X\to Y$ that is a linear homeomorphism

### Theorem
A linear bijection is an isomorphism.

### Definition
[[Banach-Mazur Distance]]

### Theorem
$X$, $Y$ normed with $Y$ complete. Then $L(X,Y)$ is complete. In particular, $X^{*}$ is complete.
#### Proof
Given $(T_{n})$ Cauchy in $L(X,Y)$:
Have $(T_{n}x)$ Cauchy in $Y$ for all $x\in X$ - since $\lVert T_{m}x-T_{n} x\rVert\leq \lVert T_{m}-T_{n} \rVert\lVert x \rVert$ so $T_{n}x\to T(x)$ for some $T(x)\in Y$.
$T$ is linear by linearity of $T_{n}$ and taking pointwise limits.
$T$ bounded: Given $\epsilon>0$ 