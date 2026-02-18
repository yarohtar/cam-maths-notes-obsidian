# Columns Property is Necessary for Partition Regularity

#ai-generated

**Proposition 15.** Let $A$ be any matrix with entries in $\mathbb{Q}$. If $A$ is PR then it must have the columns property.

**Proof.** We may assume without loss of generality that all the entries of $A$ are integers. Let the columns of $A$ be $c(1), c(2), \dots, c(n)$. For any prime $p$, colour $\mathbb{N}$ with the $d_p$ colouring. By assumption, there exists a monochromatic $x \in \mathbb{N}^n$ with $Ax = 0$, i.e. $x_1 c(1) + x_2 c(2) + \dots + x_n c(n) = 0$. Say all the $x_i$ have colour $d$.

We have a partition $B_1 \cup B_2 \cup \dots \cup B_r$ of $[n]$ given by

$L(x_i) = L(x_j)$ if $i, j \in B_s$ for some $s$;

$L(x_i) < L(x_j)$ if $i \in B_s, j \in B_t$ for some $s < t$.

For infinitely many primes $p$, say all $p \in P$, we get the same $B_1, B_2, \dots, B_r$.

Considering $Ax = 0$ performed in base $p$, we have

$\sum_{i \in B_1} d c(i) \equiv 0 \pmod{p}$ and so $\sum_{i \in B_1} c(i) \equiv 0 \pmod{p}$. But $p > \sum_{i=1}^n |c(i)|$, and so $\sum_{i \in B_1} c(i) = 0$.

From (ii), for all $s \geq 2$ we have $\sum_{i \in B_s} p^t c(i) + \sum_{i \in B_1 \cup \dots \cup B_{s-1}} x_i c(i) \equiv 0 \pmod{p^{t+1}}$ for some $t$.

We now show that $\sum_{i \in B_s} c(i) \in \langle c(j) : j \in B_1 \cup B_2 \cup \dots \cup B_{s-1} \rangle$. Suppose not. Then there exists $u \in \mathbb{Z}^m$ with $u \cdot c(i) = 0$ for all $i \in B_1 \cup B_2 \cup \dots \cup B_{s-1}$ but with $u \cdot (\sum_{i \in B_s} c(i)) \neq 0$. So $p^t u \cdot (\sum_{i \in B_s} c(i)) \equiv 0 \pmod{p^{t+1}}$, i.e. $u \cdot (\sum_{i \in B_s} c(i)) \equiv 0 \pmod{p}$ for infinitely many $p$, a contradiction.