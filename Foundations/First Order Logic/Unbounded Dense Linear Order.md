Let $\mathcal{L}=\{ < \}$ be a [[Language]]
We define DLO to be the $\mathcal{L}$-[[Theory]] with axioms:
1. $(\forall x)\  \neg(x<x)$
2. $(\forall x,y,z)\ x<y\land y<z \implies x<z$
3. $(\forall x,y)\ x\neq y\implies x<y\lor y<x$
4. $(\forall x,y)\ x<y\implies(\exists z)\ x<z<y$
5. $(\forall x)\,(\exists y,z)\ y<x<z$
## Theorem
DLO is $\aleph_{0}$-[[Categorical]].
### Proof
Back and forth argument.
Fix countable [[Model]]s $\mathcal{M},\mathcal{N}\models \mathrm{DLO}$.
Let $M=\{ a_{n}:n\geq 0 \}$ and $N=\{ b_{n}:n\geq 0 \}$.
We inductively construct a sequence of functions $(h_{n})_{n=0}^{\infty}$.
Set $h_{0}=\{ (a_{0},b_{0}) \}$.
#### Forth
First construct an order preserving bijection $h_{*}:X_{*}\to Y_{*}$.
Enumerate $X_{n}=\{ x_{1},\dots,x_{k} \}$ such that 
$$
x_{1}<^{\mathcal{M}}x_{2}<^{\mathcal{M}}<\dots<^{\mathcal{M}}x_{k}
$$
Now let $y_{i}=h_{n}(x_{i})$.
By induction hypothesis:
$$
y_{1}<^{\mathcal{N}}\dots<^{\mathcal{N}}y_{k}
$$
We define $h_{*}:=h_{n}\cup \{ (a_{n+1},b) \}$ where $b\in N$ is chosen as follows:
$$
b=\begin{cases}
y_{i} & \text{if }a_{n+1}=x_{i} \text{ for some }i\leq k  \\
u(y_{k})  & \text{if } x_{k}<^{\mathcal{M}}a_{n+1} \text{ where }y_{k}<^{\mathcal{N}}u(y_{k}) \\
l(y_{1}) & \text{if }a_{n+1}<^{\mathcal{M}}x_{1} \text{ where } l(y_{1})<^{\mathcal{N}} y_{1} \\

\end{cases}
$$

