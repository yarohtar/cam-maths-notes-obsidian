# Rado’s Theorem

#ai-generated

**Theorem 14 (Rado’s Theorem for single equations).** Let $a_1, a_2, \dots, a_n$ be non-zero rationals. Then $(a_1 a_2 \dots a_n)$ is PR if and only if $\sum_{i \in I} a_i = 0$ for some non-empty $I \subset [n]$.

**Proof.** $\Rightarrow$ is Proposition 12.

$\Leftarrow$ Given a finite colouring of $\mathbb{N}$, fix $i_0 \in I$. For suitable monochromatic $x, y$ and $z$, we shall set

$$ x_i = \begin{cases} x & \text{if } i = i_0 \\ y & \text{if } i \notin I \\ z & \text{if } i \in I - \{i_0\} \end{cases} $$

We require that $\sum a_i x_i = 0$, i.e. that $a_{i_0} x - a_{i_0} z + \sum_{i \notin I} a_i y = 0$, i.e. $\sum_{i \notin I} a_i x + y - z = 0$, and such $x, y, z$ do indeed exist by Lemma 13.