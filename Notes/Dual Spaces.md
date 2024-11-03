The dual of $X$ is $X^{*}=L(X,\mathbb{R})$ the set of all linear functionals from $X$ to $\mathbb{R}$.

[[Isomorphism of Normed Spaces]]
### Definition
For normed spaces $X$ and $Y$, an isomorphism from $X$ to $Y$ is a map $T:X\to Y$ that is a linear homeomorphism

### Theorem
For a linear bijection $T:X\to Y$ TFAE:
- $T$ is isomorphic
- $T$ and $T^{-1}$ are continuous
- there are some $c,d>0$ such that $c\lVert x \rVert\leq \lVert Tx \rVert\leq d\lVert x \rVert$


### Definition
[[Banach-Mazur Distance]]

### Theorem
$X$, $Y$ normed with $Y$ complete. Then $L(X,Y)$ is complete. In particular, $X^{*}$ is complete.
#### Proof
Given $(T_{n})$ Cauchy in $L(X,Y)$:
Have $(T_{n}x)$ Cauchy in $Y$ for all $x\in X$ - since $\lVert T_{m}x-T_{n} x\rVert\leq \lVert T_{m}-T_{n} \rVert\lVert x \rVert$ so $T_{n}x\to T(x)$ for some $T(x)\in Y$.
$T$ is linear by linearity of $T_{n}$ and taking pointwise limits.
$T$ bounded: Given $\epsilon>0$, $\lVert T_{m}-T_{n} \rVert\leq \epsilon$ for all $m,n>n_{0}$ for some $n_{0}$.
so $\lVert T_{m}x-T_{n}x \rVert\leq \epsilon \lVert x \rVert$
Let $n\to \infty$: $\lVert T_{m}x-Tx \rVert\leq \epsilon\lVert x \rVert$
Hence $\lVert Tx \rVert\leq \epsilon \lVert x \rVert+\lVert T_{m}x \rVert\leq(\epsilon+\lVert T_{m} \rVert)\lVert x \rVert$

Note that $\lVert T_{m}-T \rVert\leq \epsilon$ for all $m\geq n_{0}$ so $T_{m}\to T$. (???)
