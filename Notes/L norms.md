#### On vectors
Norms $l_p^n$ for any $1\leq p<\infty$ defined by $||X||_{p}=\left( \sum_{i=1}^{n}|X_{i}|^p \right)^{1/p}$ 

#### On sequences
Let $S$ be the space of all scalar sequences. We define the [[Normed Spaces|normed space]] 
$$
l_{p}=\left\{  X\in S \mid \sum_{i=1}^{\infty} |X_{i}|^p<\infty  \right\}
$$
With norm $||X||_{p}=\left( \sum_{i=1}^{\infty}|X_{i}|^p \right)^{\frac{1}{p}}$.

These all satisfy the desired properties by [[Minkowski's Inequality|Minkowski]] 

## Spanning
Note that $\delta_{i}=(0,\dots, 0, 1, 0,\dots, 0)$ do not span $l_{p}$ but they do span the space of finite sequences $F$. We do get close because $l_{p}$ is the closure of $F$ for $1\leq p<\infty$. 
This is FALSE for $p=\infty$, $e$.$g$. let $x=(1,1,1,\dots)$. 

Also subspacces need not be closed - eg $F$ in $l_{1}$. Even have $F$ dense in $l_{1}$.

## Dual
Want to find the [[Dual Spaces|dual space]] of $l_{p}$.
For each $y\in l_{q}$, have $\phi_{y}\in l_{p}^{*}$ with $\phi_{y}(x)=x\cdot y$.
Have $\lVert \phi_{y} \rVert\leq \lVert y \rVert_{q}$
Given $y\neq 0$ let $x_{n}=(y_{n})^{q/p}$ (the obvious choice, because we want it to converge in $l_{p}$)
So $|x_{n}$