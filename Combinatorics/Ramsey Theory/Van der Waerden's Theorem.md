For any positive integers $r, k$, there exists a smallest integer $W(r, k)$ such that if the positive integers $1, 2, \dots, n$ with $n \geq W(r, k)$ are colored with $k$ colors, then there is a monochromatic arithmetic progression of length $r$.

## Proof

We prove by induction on $r$ and $k$, ordered by the sum $r + k$.

### Base Cases

- For $r = 1$, $W(1, k) = 1$ for all $k \geq 1$, since a single element is an arithmetic progression of length $1$.
- For $k = 1$, $W(r, 1) = r$ for all $r \geq 1$, since the entire set is monochromatic.

### Inductive Step

Assume $W(r', k')$ exists for all $r' + k' < r + k$, with $r \geq 2$ and $k \geq 2$.

Let $m = W(r-1, k)$.

Divide $\{1, 2, \dots, n\}$ into blocks of length $m$:  
$B_0 = \{1, 2, \dots, m\}$,  
$B_1 = \{m+1, \dots, 2m\}$,  
$\dots$  

Each block has $m$ elements, and there are $k^m$ possible colorings of a block.

Choose $n \geq m \cdot (k^m + 1)$. By the pigeonhole principle, at least two blocks have the same coloring. Let $B_i$ and $B_j$ be such blocks with $i < j$ and identical colorings.

Let $d = j - i$.

Consider the set $S = \{x \in B_i : \text{the color of } x \text{ in } B_i \text{ equals the color of } x + d \cdot m \text{ in } B_j\}$.

Since $B_i$ and $B_j$ have identical colorings, for each color $c$, the number of elements in $B_i$ with color $c$ equals the number in $B_j$. By pigeonhole, at least one color $c$ has at least $\lceil m / k \rceil$ elements in $B_i$ with that color, and thus $|S| \geq m / k$.

$S$ is a subset of $B_i$, colored with $k$ colors. By induction, $S$ contains a monochromatic arithmetic progression of length $r-1$ in some color $c$: say $a, a + d_1, \dots, a + (r-2)d_1$, all in $S$ and color $c$.

Since $S$ consists of elements where the color matches between $B_i$ and $B_j$, the corresponding elements in $B_j$ also have color $c$: $a + d \cdot m, a + d_1 + d \cdot m, \dots, a + (r-2)d_1 + d \cdot m$.

Thus, $a, a + d \cdot m, a + d_1 + d \cdot m, \dots, a + (r-2)d_1 + d \cdot m$ form an arithmetic progression of length $r-1$ with common difference $d \cdot m$, all color $c$.

To extend to length $r$, consider $a + (r-1) d \cdot m$. Since $B_j$ has the same coloring as $B_i$, the color of $a + (r-1) d \cdot m$ in $B_j$ equals the color of $a + (r-1) d \cdot m$ in $B_i$, which is $c$ (as $a$ has color $c$ in $B_i$).

Thus, $a, a + d \cdot m, \dots, a + (r-1) d \cdot m$ is a monochromatic arithmetic progression of length $r$.

This contradicts the assumption that no such progression exists, so $W(r, k) \leq m \cdot (k^m + 1)$.

The theorem follows by induction.

## Corollary

Van der Waerden numbers exist for any finite parameters.

#ai-generated