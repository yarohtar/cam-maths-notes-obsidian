[[Convex optimisation]]
[[Lagrange multipliers]]
[[The Necessity Theorem]]
[[Duality (Optimisation)]]
[[Economist perspective]] (not important tbh)
[[Barrier method]]
[[Linear programs]]
[[Optimality conditions in LPs]]
[[Simplex method]]
[[Two-person Zero-sum Games]]
[[The Maximal Flow Problem]]
[[The Transportation Problem]]

# Main objective
Minimize functions $f:R^n\rightarrow R$
subject to $h(x)=b$ where $x \in X$

$f$ is objective function

"$h(x)=b$" is functional constraint
$x \in X$ regional constraint

If $x^*$ s.t. $f(x^*)\leq f(x)$ for all $x \in X(b)=\{x : h(x)=b, x \in X\}$
$x^*$ is called optimal
$f(x^*)$ is the optimal cost

$X(b)$ is called feasible set

If $X(b)$ is not empty then the problem is feasible

$h(x)\leq b$ is the same as $h(x)+s=b$ where $s\geq 0$

$x=(x_1,x_2\dots x_n)^T$, the coordinates of x are called decision variables.

- [[Convex optimisation]] ($f$ is convex)
- [[The Lagrange method]] (solving constrained problems)
- [[Linear programs]] ($f$ is linear, $h$ is linear)
	- simplex method to solve linear programs
- [[Application of linear programs]]