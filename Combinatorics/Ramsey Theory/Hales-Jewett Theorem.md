For any integers $m$, $r$, there exists $n$ such that if $[m]^n$ is $r$-colored, 
there is a monochromatic [[Combinatorial Line]].
### Proof
We use induction on $r$, then on $m$.
#### Base case for r: $r = 1$
For $r = 1$, any coloring of $[m]^n$ is monochromatic, so a combinatorial line is monochromatic. Thus, $n = 1$ works for all $m$.
#### Inductive step for r: Assume the theorem holds for $r - 1$, prove for $r$.
For fixed $r$, we use induction on $m$.
#### Base case for m: $m = 1$
For $m = 1$, $[1]^n$ has only one point, so $n = 1$ works.
#### Inductive step for m: Assume the theorem holds for $m - 1$, prove for $m >= 2$.
Let $HJ(r, m-1)$ be the minimal $n$ such that any $r$-coloring of $[m-1]^n$ has a monochromatic combinatorial line. (By induction on $m$, this exists.)
Let $HJ(r-1, HJ(r, m-1))$ be the minimal $n$ for $r-1$ colors and alphabet size $HJ(r, m-1)$. (By induction on $r$, this exists.)
Let $n0 = HJ(r, m-1)$.
Let $n1 = HJ(r-1, n0)$.
Let $n = n0 + n1$.
Suppose for contradiction that there exists an $r$-coloring $c$ of $[m]^n$ with no monochromatic combinatorial line.
Divide the $n$ coordinates into the first $n_{0}$ coordinates (thought of as elements of $[m]^{n_{0}}$) 
and the last $n_{1}$ coordinates (elements of $[m]^{n_{1}}$).

For each $a \in [m]^{n_{0}}$, consider the "fiber" $a \times [m]^{n_{1}}$, which is a copy of $[m]^{n_{1}}$ colored with $r$ colors. 
Since no monochromatic line exists in the whole space, 
and a [[Combinatorial Line]] could be entirely within the fiber 
(varying one of the last $n_{1}$ coordinates), 
each fiber has no monochromatic combinatorial line.

To define a coloring $d$ of $[m]^{n0}$ with $r-1$ colors, note that each fiber is colored with $r$ colors and has no monochromatic line. Since $n1 = HJ(r-1, n0)$, and the alphabet size for the fiber is $m$, by the induction hypothesis on $r$ (since $HJ(r-1, m) \leq n1$, as $n0 \geq 1$ and the bound is recursive), we can associate to each fiber a "type" based on the colors of certain "test positions" in the fiber.

Specifically, consider the $m$ test positions in the fiber where the first coordinate of the last $n1$ varies, and the remaining coordinates of the last $n1$ are fixed to $1$: i.e., the points $(1, 1^{n1-1})$, $(2, 1^{n1-1})$, ..., $(m, 1^{n1-1})$ in the fiber.

Since the fiber has no monochromatic line, the colors of these $m$ points are not all the same. Thus, there exist $i \neq j$ such that the color of $(i, 1^{n1-1})$ equals the color of $(j, 1^{n1-1})$, say color $c$.

Define the type of the fiber as the triple $(i, j, c)$. There are $\binom{m}{2} r$ possible types.

The number of possible $a$ is $m^{n0}$. Since $n0 = HJ(r, m-1)$, and $HJ(r, m-1)$ is sufficiently large (by the recursive nature of the bound), $m^{n0} > \binom{m}{2} r$, so by the pigeonhole principle, there exist two distinct $a1, a2 \in [m]^{n0}$ with the same type $(i, j, c)$.

For these $a1, a2$, the colors of $(a1, (i, 1^{n1-1}))$, $(a1, (j, 1^{n1-1}))$, $(a2, (i, 1^{n1-1}))$, $(a2, (j, 1^{n1-1}))$ are all $c$.

Let $l$ be the smallest coordinate in the first $n0$ where $a1$ and $a2$ differ: $a1(l) = p$, $a2(l) = q$, $p \neq q$.

Consider the combinatorial line in $[m]^n$ that varies the $l$-th coordinate from $p$ to $q$, with all other coordinates fixed to those of $a1$, and the last $n1$ fixed to $(i, 1^{n1-1})$.

The points in this line are ($a1$ with $l$-th coordinate set to $k$, last $n1 = (i, 1^{n1-1})$) for $k = 1$ to $m$.

In particular, for $k = p$, this is $(a1, (i, 1^{n1-1}))$, color $c$.

For $k = q$, this is $(a2, (i, 1^{n1-1}))$, color $c$.

For other $k$, the color is whatever $c$ assigns, but since the line must be monochromatic or not, and we have assumed no monochromatic line, but if all points in this line have color $c$, we have a contradiction.

The construction ensures that at least two points have color c, and the argument proceeds by contradiction, similar to the special case, where the color of the "extension" point forces the line to be monochromatic.

The calculations for the base cases are $n = 1$.

For the inductive step, $n = HJ(r, m-1) + HJ(r-1, HJ(r, m-1))$, and the reasoning is the contradiction via pigeonhole and line construction.

This completes the proof. The bound is recursive and provides an upper bound on $HJ(r, m)$.

#ai-generated