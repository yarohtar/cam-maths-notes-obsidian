$$
\frac{ \partial u }{ \partial t } =\frac{ \partial ^2u }{ \partial ^2x }\quad \quad 0\leq x\leq 1
$$
with some initial conditions $u(x,0)=u_{0}(x)$ and Dirichlet boundary conditions $u(0,t)=\phi_{0}(t)$ and $u(1,t)=\phi_{1}(t)$.

By Taylor's expansion:
$$
\begin{gather}
\frac{ \partial u }{ \partial t } =\frac{1}{k}[u(x,t+k)-u(x,t)]+O(k)\\
\frac{ \partial ^2u }{ \partial ^2x } =\frac{1}{h^2}[u(x-h,t)-2u(x,t)+u(x+h,t)]+O(h^{2})
\end{gather}
$$
So for the true solution we obtain
$$
u(x,t+k)=u(x,t)+\frac{k}{h^2}[u(x-h,t)-2u(x,t)+u(x+h,t)]+O(k^{2}+kh^{2}s)
$$
