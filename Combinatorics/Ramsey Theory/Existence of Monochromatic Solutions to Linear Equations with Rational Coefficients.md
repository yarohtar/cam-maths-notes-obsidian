# Existence of Monochromatic Solutions to Linear Equations with Rational Coefficients

#ai-generated

**Lemma 13.** Let $\lambda \in \mathbb{Q}$. Then whenever $\mathbb{N}$ is finitely coloured, there exist monochromatic $x, y$ and $z$ with $x + \lambda y = z$.

**Proof.** (cf the proof of Theorem 8.) If $\lambda = 0$ we are done; if $\lambda < 0$ we may rewrite our equation as $z - \lambda y = x$. So we may assume without loss of generality that $\lambda > 0$; say $\lambda = r/s$ with $r, s \in \mathbb{N}$.

So we need to prove that for all $k$, there exists an $n$ such that, whenever $[n]$ is $k$-coloured, there exist monochromatic $x, y$ and $z$ with $x + (r/s)y = z$.

We shall prove this by induction on $k$.

For $k = 1$, take $n = \max\{s, r + 1\}$ and $(x, y, z) = (1, s, r + 1)$.

Suppose $k > 1$. Given $n$ suitable for $k-1$, we shall show that $W(nr + 1, k)$ is suitable for $k$. Indeed, given a $k$-colouring of $[W(nr + 1, k)]$ we have a monochromatic arithmetic progression of length $nr + 1$, say $a, a + d, \dots, a + nrd$, all of colour $c$. Look at $d s, 2ds, \dots, nds$. If, say, $i ds$ has colour $c$ then we are done, as $a + (r/s) i ds = a + i r d$ and $(a, i ds, a + i r d)$ is a monochromatic triple with colour $c$. So we may assume the set $\{ds, 2ds, \dots, nds\}$ is $(k-1)$-coloured, and we are done by induction. The claim, and hence the result, follow.