For any positive integer $k$, there exists a smallest integer $S(k)$ such that if the positive integers $1, 2, \dots, n$ with $n \geq S(k)$ are colored with $k$ colors, then there is a monochromatic solution to $x + y = z$.

## Proof

By induction on $k$.

For $k=1$, trivial.

Assume for $k-1$.

Let $n = S(k-1) + S(k-1) - 1$.

Consider a coloring.

Fix $x=1$, then the pairs $(y, z)$ with $y + z = x + y$ wait, standard proof.

The set of numbers greater than $S(k-1)$ can be colored with $k-1$ colors without monochromatic Schur triple, but then find contradiction.

#ai-generated