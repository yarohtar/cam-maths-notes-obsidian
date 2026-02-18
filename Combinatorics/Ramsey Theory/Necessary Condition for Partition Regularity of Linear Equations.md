# Necessary Condition for Partition Regularity of Linear Equations

#ai-generated

**Proposition 12.** Let $a_1, a_2, \dots, a_n$ be non-zero rationals such that the matrix $(a_1 a_2 \dots a_n)$ is PR. Then $\sum_{i \in I} a_i = 0$ for some non-empty $I \subset [n]$.

**Proof.** We may assume without loss of generality that $a_1, a_2, \dots, a_n \in \mathbb{Z}$. Fix a prime $p$ with $p > \sum_{i=1}^n |a_i|$, and define a $(p-1)$-colouring of $\mathbb{N}$ by giving $x$ the colour $d_p(x)$. We know that $\sum_{i \in I} a_i x_i = 0$ for some $x_1, x_2, \dots, x_n$ all of the same colour, $d$, say. Let $L = \min \{L(x_i) : 1 \leq i \leq n\}$ and let $I = \{i : L(x_i) = L\}$. Considering $\sum_{i \in I} a_i x_i = 0$ performed in base $p$, we have $\sum_{i \in I} d a_i \equiv 0 \pmod{p}$ and so $\sum_{i \in I} a_i \equiv 0 \pmod{p}$. But $p > \sum_{i=1}^n |a_i|$, and so $\sum_{i \in I} a_i = 0$.

**Remark.** Or: for each prime $p$ we get a set $I$ with $\sum_{i \in I} a_i \equiv 0 \pmod{p}$, so some fixed set $I$ has $\sum_{i \in I} a_i \equiv 0 \pmod{p}$ for infinitely many $p$, whence $\sum_{i \in I} a_i = 0$.