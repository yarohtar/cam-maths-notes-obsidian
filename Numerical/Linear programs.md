Let $M_{1},M_{2},M_{3},N_{1},N_{2}\subseteq \mathbb{N}$ be finite sets of indices.
Let $a_{i}\in \mathbb{R}^{n}$ for $i\in M_{1}\cup M_{2}\cup M_{3}$
and let $b_{j}\in \mathbb{R}^{m}$ for $j\in N_{1}\cup N_{2}$
Finally let $c\in \mathbb{R}^{n}$ be a cost vector.
A linear program is an optimisation problem of the form:

" Minimize $c^Tx$ over $x\in \mathbb{R}^{n}$ subject to:
$a_i^Tx\leq b_i$ for $i\in M_1$
$a_i^Tx\geq b_i$ for $i\in M_2$
$a_i^Tx= b_i$ for $i\in M_3$
$x_j\geq 0$ for $j\in N_1$
$x_j\leq 0$ for $j\in N_2$ "

i.e. we are minimizing the linear function $c^{T}x$ 
over $x\in X$ 
for some $X\subseteq \mathbb{R}^{n}$ that's defined by some linear constraints.

There are other equivalent forms they can take:
[[Forms of linear programs]]
## Theorem
Suppose the set of feasible values $X$ is nonempty,
i.e. there is some $x\in \mathbb{R}^{n}$ satisfying the constraints.
Then there exists an algorithm that finds the optimal solution to the linear problem,
and this algorithm always terminates.
### Proof
[[Maximum of convex function]] is always at an [[Extreme Point]] (of domain).
So we need to find all [[Extreme Point]]s and evaluate the function there.

Consider a Linear program in standard form:
" Minimize $c^Tx$ such that $Ax=b$ and $x\geq 0$ "
where $A\in \mathbb{R}^{m\times n}$ and $x\in \mathbb{R}^n$.

We shall use a few assumptions:
- Assumption A: The rows of $A$ are linearly independent.
- Assumption B: Every set of $m$ columns of $A$ are linearly independent.
- Assumption C: All feasible [[Basic Solution|basic solutions]] are non-degenerable 
  i.e. they have exactly $m$ non-zero entries.

Select $B(1),\dots B(m)$, the non-zero entries in $x$ (do this in $n \choose m$ ways).
Set $B=[A_{B(1)} \dots A_{B(m)}]$, an $m\times m$ matrix taking columns of $A$
Now take $x_B=B^{-1}b$.
Construct a basic solution from $x_B$ by adding $0$s.

Now using [[Basic Solution#Theorem|BFS theorem]] we get the following algorithm:
1. Check all $n\choose m$ basic solutions
2. Filter out BFSs
3. Evaluate $c^Tx$ on the BFSs and output the best.

This is too slow!
To improve, we need a condition similar to [[First-order condition]]

[[Optimality conditions in LPs]]

[[Simplex method]]
