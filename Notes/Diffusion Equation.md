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
Now use $u_{m}^n=u(x_{m},t_{n})$
$$
u_{m}^{n+1}=u_{m}^{n}+\mu(u_{m-1}^n-2u_{m}^n+u_{m+1}^n)
$$
with $h=\frac{1}{M+1}$ and $\mu=\frac{k}{h^2}$ 

A method is convergent if for a fixed $\mu$ and for ever $T>0$ we have
$$
\lim_{ h \to 0 }\lvert u_{m}^n - u(x_{m},t_{n})\rvert  =0 \quad\quad \text{uniformly}
$$
### Theorem
If $\mu\leq \frac{1}{2}$ then this method converges.
#### Proof
We will use $\lVert  \rVert$ for $\lVert  \rVert_{\infty}$. 
We have 
$$
e_{m}^{n+1}=\mu e_{m-1}^n+(1-2\mu)e^n_{m}+\mu e_{m+1}^n+O(h^4)
$$
so we can get
$$
\lVert e^{n+1} \rVert \leq (2\mu+1+\lvert 1-2\mu \rvert )\lVert e^n \rVert +ch^4w
$$