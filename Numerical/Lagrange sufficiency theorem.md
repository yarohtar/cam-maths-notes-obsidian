For a problem
" Minimize $f(x)$ s.t. $h(x)=b$ and $x\in X$ "
Define:
$$L(x,\lambda)= f(x)-\lambda^T(h(x)-b)$$

If there is a point $(x^*, \lambda^*)$ s.t.:
- $L(x^*,\lambda^*)=\inf_{x\in X} L(x,\lambda^*)$, 
- $x^*$ is feasible (i.e. $x^{*}\in X$)
then $x^*$ is the solution to the original problem.

### Proof 
$\inf f(x)\leq f(x^*)$ easy
Other side:
$$
\begin{align}
\inf_{h(x)= b,\ x\in X} f(x) &= \inf_{h(x)=b,\ x\in X} f(x) - \lambda^{*T} (h(x)-b)) \\
&\geq \inf_{x\in X} f(x) - \lambda^{*T}(h(x)-b)\\
&=\inf_{x\in X} L(x,\lambda^*)=L(x^*,\lambda*)\\
&=f(x^*)
\end{align}
$$


See also [[Duality (Optimisation)]]