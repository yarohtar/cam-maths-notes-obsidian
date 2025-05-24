Consider the [[Oscillatory Integrals]]:
$$
F(x)=\int_{a}^{b}f(t)e^{ix\phi(t)}dt
$$
where $\phi$ is stationary at a point $c\in(a,b)$.
Suppose that $\phi''(c)\neq0$

# Method
## Taylor expand
Write:
$$
\phi(t) = \phi(c) + \frac{\phi''(c)}{2} + \dots
$$
## Separate into sections
Let $\epsilon>0$ be small (but will depend on $x$)
By [[Oscillatory Integrals with monotonic phase]], 
we know that in the areas of monotonic $\phi$ 
we have $O\left( \frac{1}{x} \right)$ contribution.
Thus we can write:
$$
F(x) = \int_{c-\epsilon}^{c+\epsilon} f(t) e^{ix\phi(t)} dt + O\left( \frac{1}{x} \right)
$$
## Use substitution
Substitute $s^{2}=-\frac{x\phi''(c)(t-c)^{2}}{2}$ 