# Gallai’s Theorem

#ai-generated

**Theorem 11 (Gallai’s Theorem).** For any finite $S \subset \mathbb{N}^d$ and any $k$-colouring of $\mathbb{N}^d$, there exists a monochromatic homothetic copy of $S$.

**Proof.** Let $S = \{S(1), S(2), \dots, S(m)\}$. Given a $k$-colouring $c$ of $\mathbb{N}^d$, define a $k$-colouring $c_0$ of $[m]^n$ ($n$ large) by $c_0 (x) = c( \sum_{i=1}^n S(x_i) )$. By Hales-Jewett, there is a monochromatic line, giving a monochromatic homothetic copy of $S$ (with $\lambda$ the number of active coordinates).

**Remarks.** 1. Or by a product argument and focussing. 2. For $S = \{(x, y) : x, y \in \{0, 1\}\}$, Gallai’s Theorem tells us that there exists a monochromatic square. Could we have used 2-parameter Hales-Jewett instead?—No, this would only give us a rectangle.