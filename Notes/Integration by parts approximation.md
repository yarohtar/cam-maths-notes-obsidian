$$
\int_{a}^b fg^{(n)}dt=\sum_{k=1}^n(-1)^{k-1}[f^{(k-1)}g^{(n-k)}]+(-1)^n\int_{a}^b f^{(n)}gdt
$$
the boundary terms can give an [[Asymptotic Approximation]] under certain circumstances
### Example
$F(x)=\int_{x}^\infty e^{-t^2/2}dt$ as $x\to \infty$.
$$
\begin{align}
F(x) & =\int_{x}^\infty \frac{te^{-t^2/2}}{t}dt \\
 & =\left[ -\frac{1}{t}e^{-t^2/2} \right]_{x}^\infty+\int_{x}^\infty \frac{e^{-t^{2}/2}}{t^{2}}dt \\
 & =\frac{e^{-x^{2}/2}}{x}+\dots
\end{align}
$$
Need to show that $\text{error}=o\left( \frac{e^{-x^{2}/2}}{x} \right)$
Can show $\text{error}\leq \frac{e^{-x^{2}/2}}{x^{3}}$ as $x\to \infty$
So $F(x)\sim \frac{e^{-x^{2}/2}}{x}$ as $x\to \infty$

We can keep integrating by parts to find
$$
F(x)\sim \frac{e^{-x^{2}/2}}{x}\sum_{n}(-1)^n \frac{(2n-1)!!}{x^{2n}}
$$
(this diverges ...)
### Example
