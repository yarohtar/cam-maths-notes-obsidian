We consider 
$$
u_{t}=u_{x}
$$
for $t\geq 0$ and $x\in \mathbb{R}$
with initial condition $u(x,0)=\phi(x)$.
Note that this has exact solution $u(x,t)=\phi(x+t)$

## Downward instability
Consider the [[Semidiscretization]]:
$$
\frac{\partial u_{m}(t)}{\partial t} = \frac{1}{h} (u_{m}(t)-u_{m-1}(t))
$$
using the [[Euler method]]:
$$
u_{m}^{n+1}=u_{m}^{n}+\mu(u_{m}^{n}-u_{m-1}^{n})
$$
for $n\in \mathbb{Z}_{+}$
We use [[Fourier Analysis of Stability]]:
$$
H(\theta)=1+\mu-\mu e^{-i\theta}
$$
But then $\left\lvert  H\left( \frac{\pi}{2} \right)  \right\rvert ^{2} =(1+\mu)^{2}+\mu^{2}>1$ 
so the method is unstable for all $\mu>0$
## Upwind scheme
Consider the [[Semidiscretization]]:
$$
\frac{\partial u_{m}(t)}{\partial t} = \frac{1}{h} (u_{m+1}(t)-u_{m}(t))
$$
using the [[Euler method]]:
$$
u_{m}^{n+1} = u_{m}^{n} + \mu(u_{m+1}^{n}-u_{m}^{n})
$$
for $n\in \mathbb{Z}_{+}$
This is veery similar to the previous bit, but now:
$$
H(\theta)=1-\mu+\mu e^{i\theta}
$$
So $\lvert H(\theta) \rvert =\lvert 1-\mu+\mu e^{i\theta} \rvert \leq \lvert 1-\mu \rvert+\mu=1$ for $\mu \in[0,1]$.
Hence we have stability for $\mu\leq 1$, but instability for $\mu>1$
## Leap-frog method
We [[Semidiscretization]] as
$$
\frac{\partial u_{m}}{\partial t} = \frac{1}{2h} (u_{m+1}(t)- u_{m-1}(t))
$$
But now we solve the ODE using the midpoint rule:
$$
y_{n+1}=y_{n-1}+2kf(t_{n},y_{n})
$$
We find the two-step leapfrog method:
$$
u_{m}^{n+1}=\mu(u_{m+1}^{n}-u_{m-1}^{n}) + u_{m}^{n-1}
$$
The local error is $O(k^{3}+kh^{2})=O(h^{3})$
We use [[fouri]]