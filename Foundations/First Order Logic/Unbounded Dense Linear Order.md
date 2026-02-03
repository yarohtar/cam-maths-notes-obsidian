Let $\mathcal{L}=\{ < \}$ be a [[Language]]
We define DLO to be the $\mathcal{L}$-[[Theory]] with axioms:
1. $(\forall x)\  \neg(x<x)$
2. $(\forall x,y,z)\ x<y\land y<z \implies x<z$
3. $(\forall x,y)\ x\neq y\implies x<y\lor y<x$
4. $(\forall x,y)\ x<y\implies(\exists z)\ x<z<y$
5. $(\forall x)\,(\exists y,z)\ y<x<z$
### Theorem
DLO is $\aleph_{0}$-[[Categorical]].
#### Proof
Back and forth argument.
Fix countable [[Model]]s $\mathcal{M},\mathcal{N}\models \mathrm{DLO}$.
Let $M=\{ a_{n}:n\geq 0 \}$ and $N=\{ b_{n}:n \}$
