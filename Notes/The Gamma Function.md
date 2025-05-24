The Gamma function is an analytic way to represent factorials.
$$
\Gamma(\xi)=\int_{0}^\infty t^{\xi-1}e^{-t}dt
$$
This is analytic for $\mathrm{Re}(\xi)>0$.
It satisfies the functional equation:
$$
z\Gamma(z)=\Gamma(z+1)
$$
(as expected)
Also $\Gamma(1)=1$ so $\Gamma(n+1)=n!$ for $n\in \mathbb{N}$
For $x>0$, by simple substitution we find:
$$
\int_{0}^\infty t^{\xi-1}e^{-xt}dt=\frac{\Gamma(\xi)}{x^{\xi}}
$$
### Reflexion formula
$$
\Gamma(z)\Gamma(1-z)= \frac{\pi}{\sin \pi z}
$$
### Duplication formula
$$
\Gamma(z)\Gamma\left( z+\frac{1}{2} \right) = 2^{1-2z} \sqrt{ \pi } \Gamma(2z)
$$
### Useful integral
$$
\int_{0}^{\inf} e^{-ax}
$$
### Properties
- $\Gamma(\xi+1)=\xi \Gamma(\xi)$
- $\Gamma(n+1)=n!$
- $\int_{0}^\infty t^{\xi-1}e^{-xt}dt=\frac{\Gamma(\xi)}{x^{\xi}}$ for $x>0$
- Generalizes the binomial coefficients: 
$$
{\xi \choose k}=\frac{1}{k!} \frac{\Gamma(\xi+1)}{\Gamma(\xi-k+1)} 
$$
for $k=0,1,\dots$  and $\xi \in \mathbb{C}$
- $(1+t)^{\xi}=\sum_{k=0}^{\infty}{\xi \choose k}t^k$


