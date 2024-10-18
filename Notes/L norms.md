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
Have $\lVert \phi_{y} \rVert\leq \lVert y \rVert_{q}$ ([[Hölder inequality]])

### Norm of $\phi_y$
Given $y\neq 0$ let $x_{n}=(y_{n})^{q/p}$ (the obvious choice, because we want it to converge in $l_{p}$)

So $|x_{n}|^p=|y_{n}|^q$ so $x\in l_{p}$ with $\lVert x \rVert_{p}=\left( \sum|y_{n}|^q \right)^{1/p}=\lVert y \rVert_{q}^{q/p}$

Have $\phi_{y}(x)=x\cdot y=\sum(y_{n})^{q/p+1}=\sum(y_{n})^q=\lVert y \rVert_{q}^q$ 
($\frac{q}{p}+1=q$ because $\frac{1}{p}+\frac{1}{q}=1$)

So $\lVert \phi_{y} \rVert\geq \frac{\lVert y \rVert_{q}^q}{\lVert y \rVert_{q}^{q/p}}=\lVert y \rVert_{q}$
Hence $\lVert \phi_{y} \rVert=\lVert y \rVert_{q}$

### Theorem
The map $\theta:l_{q}\to l_{p}^{*}$ is an isometric isomorphism (ie they are the same)
#### Proof
$\theta$ linear, as $\phi_{\lambda y+\mu y'}=\lambda \phi_{y}+\mu \phi_{y'}$
$\theta$ isometry as $\lVert \phi_{y} \rVert=\lVert y \rVert_{q}$ (so $\theta$ is injective)
Need $\theta$ surjective
Given $T\in l_{p}^{*}$ let $y_{n}=Tl_{n}$ each 1 
want $y\in l_{q}$ and $T=\phi_{y}$
For some fixed $N$, let:
$$
x_{n}=\begin{cases}
|y_{n}|^{q/p}sgn (y_{n}) & n\leq N \\
0 & n>N
\end{cases}
$$
Then $x \in l_{p}$ with $\lVert x \rVert_{p}=\left( \sum_{n=1}^{N}|y_{n}|^q \right)^{1/p}$
Also $Tx=\sum_{n=1}^{N}|y_{n}|^q\leq \lVert T \rVert\left( \sum_{n=1}^{N}|y_{n}|^q \right)^{1/p}$
ie $\left( \sum_{n=1}^{N}|y_{n}|^q \right)^{1-1/p}\leq \lVert T \rVert$ so $y\in l_{q}$ with $\lVert y \rVert_{q}\leq \lVert T \rVert$ as $N$ is arbitrary
Finally $\phi_{y}=T$ on $l_{n}$ for all $n$
so $\phi _y=T$ on $<l_{n}:n\in \mathbb{N}>$ (notation for linear span)
$\phi_{y}T$ is linear and continuous
ie $\phi_{y}=T$ on the whole of $l_{p}$.