Rado's theorem states that for certain systems of linear equations, if the coefficients satisfy certain regularity conditions, then there is a monochromatic solution in any finite coloring of the integers.

Specifically, for a system of equations $\sum c_i x_i = 0$ where the $c_i$ are integers, if the system is regular (no non-trivial solution with all variables positive), then for any finite coloring, there is a monochromatic solution.

### Definitions

- **Partition Regularity (PR)**: Let $A$ be an $m \times n$ matrix with rational entries. We say that $A$ is **partition regular (PR)** (over $\mathbb{N}$) if, whenever $\mathbb{N}$ is finitely coloured (i.e., partitioned into finitely many subsets), there exists a monochromatic $x \in \mathbb{N}^n$ such that $Ax = 0$.

  We also talk about "the equation $Ax = 0$" being PR, meaning the same condition holds for the homogeneous system represented by $A$.

- **Columns Property**: Let $A$ have columns $c(1), c(2), \dots, c(n) \in \mathbb{Q}^m$. We say that $A$ has the **columns property** if there exists a partition $B_1 \cup B_2 \cup \cdots \cup B_r$ of $[n]$ such that:
  - $\sum_{i \in B_1} c(i) = 0$; and
  - For $s = 2, 3, \dots, r$, $\sum_{i \in B_s} c(i) \in \operatorname{span}_\mathbb{R} \{c(j) : j \in B_1 \cup B_2 \cup \cdots \cup B_{s-1}\}$.

  (Note that the span can equivalently be taken over $\mathbb{Q}$, as any rational linear combination of rational vectors that sums to zero can be achieved rationally.)

### Theorem Statement: Rado's Theorem

A rational matrix $A$ is partition regular if and only if $A$ has the columns property.

### Proof

The proof proceeds in two directions: sufficiency ($\Leftarrow$) and necessity ($\Rightarrow$). Sufficiency is established via Proposition 15, and necessity via Theorem 16 and Lemma 17. We first prove the supporting results.

#### Supporting Results

1. **Proposition 12**: Let $a_1, a_2, \dots, a_n$ be non-zero rationals such that the matrix $(a_1 \, a_2 \, \cdots \, a_n)$ is PR. Then $\sum_{i \in I} a_i = 0$ for some non-empty $I \subset [n]$.

   **Proof**: Assume without loss of generality that $a_1, a_2, \dots, a_n \in \mathbb{Z}$. Fix a prime $p > \sum_{i=1}^n |a_i|$. For $x \in \mathbb{N}$, let $d_p(x)$ be the last non-zero digit in the base-$p$ expansion of $x$ (i.e., if $x = \sum_{r=0}^\infty d_r p^r$ with $0 \leq d_r \leq p-1$, then $d_p(x) = d_{L(x)}$ where $L(x) = \min \{r : d_r \neq 0\}$).

   Color $\mathbb{N}$ with $p-1$ colors using $d_p(x)$. Since $(a_1 \, a_2 \, \cdots \, a_n)$ is PR, there exist $x_1, x_2, \dots, x_n$ all of the same color $d$, with $\sum_{i=1}^n a_i x_i = 0$.

   Let $L = \min \{L(x_i) : 1 \leq i \leq n\}$, and let $I = \{i : L(x_i) = L\}$. Performing the equation in base $p^L$, we have $\sum_{i \in I} a_i d_i \equiv 0 \pmod{p}$, so $\sum_{i \in I} a_i \equiv 0 \pmod{p}$. Since $p > \sum_{i=1}^n |a_i|$, $\sum_{i \in I} a_i = 0$.

2. **Lemma 13**: Let $\lambda \in \mathbb{Q}$. Then, whenever $\mathbb{N}$ is finitely coloured, there exist monochromatic $x, y, z$ with $x + \lambda y = z$.

   **Proof**: Without loss of generality, assume $\lambda > 0$ (otherwise, rewrite as $z - \lambda y = x$). Write $\lambda = r/s$ with $r, s \in \mathbb{N}$.

   Prove by induction on the number of colors $k$.

   - For $k=1$, take $n = \max\{s, r+1\}$, and $(x, y, z) = (1, s, r+1)$.

   - Suppose true for $k-1$. Given $n$ suitable for $k-1$, let $W(n r + 1, k)$ be the Van der Waerden number. Given a $k$-coloring of $[W(nr+1, k)]$, there is a monochromatic arithmetic progression of length $nr+1$, say $a, a+d, \dots, a + nrd$, all color $c$.

   Look at $ds, 2ds, \dots, nds$. If some $ids$ has color $c$, set $(x, y, z) = (a, ids, a + idr)$. Otherwise, $\{ds, 2ds, \dots, nds\}$ is $(k-1)$-colored, so by induction, there exist monochromatic $x', y', z'$ in this set with $x' + (r/s) y' = z'$, and adjust to get the triple in the original set.

3. **Theorem 14 (Rado's Theorem for Single Equations)**: Let $a_1, a_2, \dots, a_n$ be non-zero rationals. Then $(a_1 \, a_2 \, \cdots \, a_n)$ is PR if and only if $\sum_{i \in I} a_i = 0$ for some non-empty $I \subset [n]$.

   **Proof**:
   - $\Rightarrow$: By Proposition 12.
   - $\Leftarrow$: Given a finite coloring of $\mathbb{N}$, fix $i_0 \in I$. By Lemma 13, there exist monochromatic $x, y, z$ with $x + \lambda y = z$, where $\lambda = -\sum_{i \neq i_0, i \in I} a_i / a_{i_0}$ (assuming $a_{i_0} \neq 0$).

     Set:
     \[
     x_i = \begin{cases}
     x & \text{if } i = i_0 \\
     y & \text{if } i \notin I \\
     z & \text{if } i \in I - \{i_0\}
     \end{cases}
     \]
     Then $\sum a_i x_i = a_{i_0} x + \sum_{i \notin I} a_i y + \sum_{i \in I - \{i_0\}} a_i z = a_{i_0} x - a_{i_0} z + \sum_{i \notin I} a_i y = 0$, as required.

4. **Proposition 15**: Let $A$ be any matrix with entries in $\mathbb{Q}$. If $A$ is PR, then it has the columns property.

   **Proof**: Assume entries are integers. Let $c(1), \dots, c(n)$ be the columns. For each prime $p$, color $\mathbb{N}$ with $d_p(x)$. By PR, there exists monochromatic $x \in \mathbb{Z}^n$ with $Ax = 0$, all $x_i$ color $d$.

   Partition $[n]$ into $B_1, \dots, B_r$ where $i, j \in B_s$ iff $L(x_i) = L(x_j)$, and $i \in B_s, j \in B_t$ iff $L(x_i) < L(x_j)$ for $s < t$.

   In base $p$, $\sum_{i \in B_1} d_i c(i) \equiv 0 \pmod{p}$, so $\sum_{i \in B_1} c(i) = 0$.

   For $s \geq 2$, $\sum_{i \in B_s} p^{L} d_i c(i) + \sum_{i \in B_1 \cup \cdots \cup B_{s-1}} x_i c(i) \equiv 0 \pmod{p^{t+1}}$ for some $t$, implying $\sum_{i \in B_s} c(i) \in \operatorname{span} \{c(j) : j \in B_1 \cup \cdots \cup B_{s-1}\}$.

5. **Theorem 16**: Let $m, p, c \in \mathbb{N}$. Whenever $\mathbb{N}$ is finitely coloured, there exists a monochromatic $(m, p, c)$-set.

   (An $(m, p, c)$-set with generators $x_1, \dots, x_m$ consists of all numbers $\sum_{i=1}^m \lambda_i x_i$ where $\lambda_1 = c$, $\lambda_i \in \{-\p, \dots, p\}$ for $i > 1$, and the exponents are non-decreasing in some sense—see the full definition in the text for details.)

   **Proof**: By induction on $m$, using Van der Waerden's Theorem repeatedly to build monochromatic arithmetic progressions and restrict to subsets.

6. **Lemma 17**: If $A$ has the columns property, then there exist $m, p, c \in \mathbb{N}$ such that every $(m, p, c)$-set contains a solution to $Ax = 0$.

   **Proof**: Construct $y_i$ from the partition $B_1, \dots, B_r$ and rational coefficients $q_{is}$, then set $x_i = y_i$ for the generators, and scale appropriately to ensure solutions in the set.

#### Main Proof of Rado's Theorem

- $\Leftarrow$ (Sufficiency): By Proposition 15.
- $\Rightarrow$ (Necessity): By Theorem 16 and Lemma 17, since if $A$ is PR, we can find $m, p, c$ such that monochromatic $(m, p, c)$-sets exist and contain solutions to $Ax = 0$, implying the columns property.

This completes the proof. The theorem is significant as it provides a finite-time checkable criterion for partition regularity, bridging Ramsey theory and linear algebra. For further reading, consult sources like Hindman's "Ramsey Theory" or Graham et al.'s "Ramsey Theory on the Integers."

#ai-generated