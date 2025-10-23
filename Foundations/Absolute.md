Let $M$ and $N$ be [[Structure]]s for a [[Language]] $\mathcal{L}$ such that $M\subseteq N$
Let $\phi$ be a formula in $n$ [[Free Variable]]s.
We say that $\phi$ is absolute between $M$ and $N$ if 
it is [[Upwards Absolute]] and [[Downwards Absolute]] i.e.
$$
\forall x_{1},\dots,x_{n} \in M\quad %quad
M\models\phi(x_{1},\dots,x_{n}) \iff N\models\phi(x_{1},\dots,x_{n})
$$
where we use $M\models \phi$ to mean $\phi$ is [[Satisfied]] in $M$

## Theorem
If $M$ is a [[Substructure]] of $N$, 
then all quantifier free formulas are absolute between $M$ and $N$

### Example
Language of set theory has symbols $\{ \in \}$
Take
$$
\varepsilon_{0}(x) := (\forall z)(\neg z \in x)
$$
meaning $x=\varnothing$
Also take
$$
\varepsilon_{1}(x):=(\forall z)(z\in x \implies \varepsilon_{0}(z))
$$
meaning $x=\{ \varnothing \}$

Take a model
$$
M\models ZFC
$$
Let $m$ be such that $M\models\varepsilon_{0}(m)$ (exists by [[Empty-set axiom]])
and $n$ such that $M\models\varepsilon_{1}(n)$ (exists by [[Pair-set axiom]] ...)
Then take $N=M\setminus\{ m \}$
But then $N\models\varepsilon_{0}(n)$ !!
and thus $\varepsilon_{0}$ is not absolute in the [[Language]] of set theory.
