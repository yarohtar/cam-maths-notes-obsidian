For any positive integer $k$, there exists a smallest integer $S(k)$ such that if the positive integers $1, 2, \dots, n$ with $n \geq S(k)$ are colored with $k$ colors, then there is a monochromatic solution to $x + y = z$.

## Proof

By induction on $k$.

### Base Case: $k = 1$

For $k = 1$, consider the set $\{1, 2, 3\}$. In any 1-coloring (i.e., all elements the same color), we have $1 + 2 = 3$. Thus, $S(1) = 3$.

### Inductive Step

Assume $S(k-1)$ exists, and prove $S(k) \leq 2 \cdot S(k-1) + 1$.

Let $m = S(k-1)$. We will show that any $k$-coloring of $\{1, 2, \dots, 2m + 1\}$ contains a monochromatic solution to $x + y = z$ with $x$, $y$, $z$ distinct.

Suppose for contradiction that there exists a $k$-coloring $c$ of $\{1, 2, \dots, 2m + 1\}$ with no monochromatic $x + y = z$ (with $x < y < z$ to ensure distinctness, as $x + y = z$ implies $z > y > x$).

Let $A = \{x \in \{1, 2, \dots, 2m + 1\} \mid x > m\} = \{m+1, m+2, \dots, 2m+1\}$. Note that $|A| = m$.

For each color class $C$ (i.e., the set of elements assigned color $C$), $|C \cap A| \leq 1$. This is because if $x, y \in C \cap A$ with $x < y$, then $x + y \geq (m+1) + (m+2) = 2m + 3 > 2m + 1$, so $x + y$ is not in the set $\{1, 2, \dots, 2m + 1\}$, and thus cannot equal any $z$ in the set.

There are $k$ color classes, and $|A| = m$. By the pigeonhole principle, the average number of elements from $A$ per color class is $m / k$. Since $m \geq S(k-1) \geq 3$ for $k \geq 2$, and $k \geq 2$, we have $m > k$ (for $k=2$, $m=3 > 2$; for $k=3$, $m \geq 5 > 3$; and so on, as $S(k-1)$ grows rapidly). Thus, $\lceil m / k \rceil \geq 2$.

Therefore, some color class $C$ has at least $\lceil m / k \rceil \geq 2$ elements in $A$, contradicting the fact that $|C \cap A| \leq 1$.

Hence, no such $k$-coloring exists, so $S(k) \leq 2m + 1 = 2 \cdot S(k-1) + 1$.

By induction, $S(k)$ exists for all $k$.

## Remarks

- This proof provides an upper bound on $S(k)$, but the actual minimal $S(k)$ (known as Schur numbers) are smaller in many cases (e.g., $S(2) = 5$, $S(3) = 14$, $S(4) = 45$, $S(5) = 161$).
- The proof relies on the pigeonhole principle and the inductive hypothesis to force a contradiction.
- For $k \geq 2$, the condition $m > k$ ensures the pigeonhole argument works, as $\lceil m / k \rceil \geq 2$.

#ai-generated