We consider the diffusion equation
$$
\frac{\partial u}{\partial t} = \frac{\partial^{2}u}{\partial x^{2}}
$$
where $-\infty<x<\infty$ and $t\geq 0$
We assume a recurrence of the form:
$$
\sum_{k=r}^{s}a_{k}u_{m+k}^{n+1}=\sum_{k=r}^{s}b_{k}u_{m+k}^{n}
$$
where $m\in \mathbb{Z}$
## Fourier analysis of stability
[[Fourier Analysis of Stability]]
### Euler
$$
u_{m}^{n+1} = u_{m}^{n} + \mu(u_{m-1}^{n}-2u_{m}^{n}+u_{m+1}^{n})
$$
has amplification factor:
$$
H(\theta) = 1+\mu(e^{-i\theta}-2+e^{i\theta}) = 1- 4\mu \sin ^{2} \frac{\theta}{2} \in [1-4\mu,1]
$$
this the method is stable iff $\mu\leq \frac{1}{2}$
