### Example
Consider $I(x)=\int_{0}^\infty \frac{e^{-t}}{1+xt}dt$
We want to understand the integral behaviourr as $x\to 0^+$.

Taylor series of $\frac{1}{1+xt}$ is $\sum_{n=0}^{\infty}(-1)^nx^nt^n$ ehhhh
Better to consider:
$$
\sum_{n=0}^{N} (-xt)^n=\frac{1}{1+xt} - r_{N}
$$
where $r_{N}=\frac{(-xt)^{N+1}}{1+xt}$.

$$
\begin{align}
I(x) & =\int _{0}^\infty\left( \sum ^N(-1)^nx^nt^n+r_{N} \right)e^{-t} \, dt  \\
 & =\sum_{n=0}^N(-1)^nx^n\left[ \int \right]
\end{align}
$$