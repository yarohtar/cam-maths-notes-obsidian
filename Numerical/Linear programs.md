Let $M_{1},M_{2},M_{3},N_{1},N_{2}\subseteq \mathbb{N}$ be finite sets of indices.
Let $a_{i}\in \mathbb{R}^{n}$ for $i\in M_{1}\cup M_{2}\cup M_{3}$
and let $b_{i}\in \mathbb{R}$
Minimize $c^Tx$ subject to:
$a_i^Tx\leq b_i$ for $i\in M_1$
$a_i^Tx\geq b_i$ for $i\in M_2$
$a_i^Tx= b_i$ for $i\in M_3$
$x_j\geq 0$ for $j\in N_1$
$x_j\leq 0$ for $j\in N_2$

Let $A$ be a $\mathbb{R}^{m\times n}$ matrix.
Let $b\in \mathbb{R}^{m}$ and $c\in \mathbb{R}^{n}$ be vectors
The linear program takes the following general form:
" Minimize $c^Tx$ over $x\in \mathbb{R}^{n}$ subject to $Ax\leq b$. "

There are other equivalent forms they can take:
[[Forms of linear programs]]
## Solving the linear program

[[Maximum of convex function]] is always at an [[Extreme Point]] (of domain).

So if we found all extreme points and evaluated the function there, 
we should have our solution.

Consider a Linear program in standard form:
minimize $c^Tx$ such that $Ax=b$ and $x\geq 0$ 
where $A\in \mathbb{R}^{m\times n}$ and $x\in \mathbb{R}^n$.

We shall use a few assumptions:
- Assumption A: The rows of $A$ are linearly independent.
- Assumption B: Every set of $m$ columns of $A$ are linearly independent.
- Assumption C: All feasible [[Basic solutions (LP)|basic solutions]] are non-degenerable 
  i.e. they have exactly $m$ non-zero entries.

Select $B(1),\dots B(m)$ the non-zero entries in $x$ (do this in $n \choose m$ ways).
Set $B=[A_{B(1)} \dots A_{B(m)}]$, an $m\times m$ matrix taking columns of $A$
Now take $x_B=B^{-1}b$.
Construct a basic solution from $x_B$ by adding $0$s.

Now using [[Basic solutions (LP)#Theorem|BFS theorem]] we get the following algorithm:
1. Check all $n\choose m$ basic solutions
2. Filter out BFSs
3. Evaluate $c^Tx$ on the BFSs and output the best.

This is too slow!
To improve, we need a condition similar to [[First-order condition]]

[[Optimality conditions in LPs]]

[[Simplex method]]
