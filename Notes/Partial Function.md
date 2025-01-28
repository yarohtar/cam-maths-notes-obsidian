Write $f:X\dashrightarrow Y$ for partial functions from $X$ to $Y$. This means that not all inputs in $X$ have an output in $Y$. We write $dom(f)$ for the set of values which does have an output in $Y$.
We also write:
$$
\begin{align}
f(x)\downarrow \quad %quad
\quad %quad
 & \text{iff } x\in dom(f)  \\
f(x)\uparrow \quad %quad
\quad %quad
 & \text{otherwise}
\end{align}
$$
and use terminology that $f$ converges or diverges on input $x$.

### Definition
Let $F:\mathbb{B}^{n+1}\dashrightarrow \mathbb{B}^{n+1}$ be any partial function. We say that a [[Register Machine]] $M$ performs the operation $F$ if for all $\vec{w}\in \mathbb{B}^{n+1}$:
1. If $F(\vec{w})\downarrow=\vec{v}$ then $M$ converges on input $\vec{w}^{+}$ with register content $\vec{v}^{+}$
2. If $F(\vec{w})\uparrow$ then $M$ diverges on input $\vec{w}^{+}$
(Note that we used the $^{+}$ to indicate padding for scratch space that the register machine may use for memory purposes. I will omit that padding in my notes going forward.)