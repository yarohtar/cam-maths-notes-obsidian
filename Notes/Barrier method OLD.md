We want to minimize $f(x)$ subject to $f_i(x)\leq 0$ for $i=1\dots m$ 
Given that $f$, and all $f_i$ are [[Convex Function]], we have that $\{x : f_i(x)\leq 0 \text{ for all } i\}$ is also [[Convex Set]].

Now consider the function $f(x) + \sum_{i=1}^m \phi(f_i(x))$ where $\phi(x)=0$ for $x\leq0$ and $\phi(x)=\infty$ for $x>0$.
This function has the same minimum. However, it is not differentiable anymore. 
Instead take $\phi (x) = -\log(-x)$ (this is called the logarithmic barrier function).

Now we look at the problem $\min(tf(x)+\Phi(x))$ for different values of $t$, where $\Phi(x)=\sum_{i=1}^m\phi(f_i(x))$

#### The algorithm:
1. Initialize the algorithm from $x_0$ in the interior of feasible set. Set $t=t_0$
2. Repeat the following
	1. Minimize $t_0 f(x) + \Phi(x)$ (using your favourite convex optimisation method)
	2. Stop the algorithm if $t_0$ is large
	3. Change $t_0$ to $\alpha t_0$ where $\alpha$ is a fixed number $>1$

This was all assuming $\Phi$ was convex. We can calculate it's gradient and hessian:
$$\Phi(x)=-\sum_{i=1}^m\log(-f_i(x))$$
$$\nabla\Phi(x) = -\sum_{i=1}^m \frac{\nabla f_i(x)}{f_i(x)}$$
$$\nabla^2 \Phi(x) = \sum_{i=1}^m \frac{\nabla f_i(x)\nabla f_i(x)^T}{f_i(x)^2} + \frac{\nabla^2 f_i(x)}{f_i(x)}\succeq 0$$
