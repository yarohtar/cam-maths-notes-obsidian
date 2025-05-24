We have an integral of the form
$$
F(x) = \int_{a}^{b} e^{x\phi(t)} dt
$$
and we want to find [[Asymptotic Approximation]] of $F$ 
when $x\to \infty$
# The method
## Draw picture of $\phi(t)$
We want to figure out the most important features of $\phi$ 
## Find the significant points
We want to find all the global maxima of $\phi$.
This may include local maxima in $(a,b)$ 
as well as the endpoints $a$ and $b$
## Truncation
We split the integral into small sections around the maxima
## Expansion
For each maximum $c$, write:
$$
x\phi(t) \sim x\phi(c) + xA_{p}(t-c)^{p} + xA_{p+1}(t-c)^{p+1} + \dots
$$
up to appropriate number of terms. 
Note that we take $A_{n}=\phi^{(n)}(c)$ and $p$ is the 
## Change variables
