# The Hales-Jewett Theorem

#ai-generated

**Theorem 9 (The Hales-Jewett Theorem).** Let $m, k \in \mathbb{N}$. Then there exists $n \in \mathbb{N}$ such that whenever $[m]^n$ is $k$-coloured there exists a monochromatic line.

**Remarks.** 1. The smallest such $n$ is denoted by $HJ(m, k)$.

2. The Hales-Jewett Theorem implies Van der Waerden's Theorem—we need only embed a Hales-Jewett cube of sufficiently high dimension linearly into $\mathbb{N}$, and so that the embedding is injective on lines. For example, given a $k$-colouring $c$ of $\mathbb{N}$, induce a $k$-colouring $c_0$ of $[m]^n$ ($n$ large) by $c_0 ((x_1 , x_2 , \dots , x_n )) = c(x_1 + x_2 + \cdots + x_n )$. By Hales-Jewett, there is a monochromatic line, and this corresponds to a monochromatic arithmetic progression of length $m$ in $\mathbb{N}$. So we should regard the Hales-Jewett theorem as an abstract version of Van der Waerden's Theorem.

If $L$ is a line in $[m]^n$ write $L^-$ and $L^+$ for its first and last points (in the ordering on $[m]^n$ given by $x \leq y$ if $x_i \leq y_i$ for all $i$). Lines $L_1 , L_2 , \dots , L_k$ are focussed at $f$ if $L^+_i = f$ for all $i$. They are colour-focussed (for a given colouring) if in addition each $L_i - \{L^+_i \}$ is monochromatic, no two the same colour.

**Proof (of Theorem 9).** By induction on $m$; the case $m = 1$ is trivial. Given $m > 1$, we may assume that $HJ(m - 1, k)$ exists for all $k$. We make the following claim: For all $r \leq k$, there exists $n$ such that whenever $[m]^n$ is $k$-coloured, there exists EITHER a monochromatic line OR $r$ colour-focussed lines. The result will follow immediately from this claim—put $r = k$ and look at the focus. The proof of the claim is by induction on $r$. For $r = 1$ we may take $n = HJ(m - 1, k)$.

Given $n$ suitable for $r$, we shall show that $n + HJ(m - 1, k^m )$ is suitable for $r + 1$. Write $n_0 = HJ(m - 1, k^m )$.

Given a $k$-colouring of $[m]^{n+n_0}$ with no monochromatic line, identify $[m]^{n+n_0}$ with $[m]^n \times [m]^{n_0}$. There are $k^{m}$ ways to colour a copy of $[m]^{n_0}$. So by our choice of $n_0$, we have a line $L$ in $[m]^{n_0}$, say with active coordinate set $I$, such that for all $a \in [m]^{n_0}$ and all $b, b' \in L^- - \{L^+ \}$, we have $c(a, b) = c(a, b') = c_0(a)$, say. Now by definition of $n$, there exist $r$ colour-focussed lines for $c_0$, say $L_1, L_2, \dots, L_r$, with active coordinate sets $I_1, I_2, \dots, I_r$ respectively, and focus $f$.

But now let $L'_i$ be the line through the point $(L^-_i, L^+)$ with active coordinate set $I_i \cup I$ ($i = 1, 2, \dots, r$). Then $L'_1, L'_2, \dots, L'_r$ are colour-focussed at $(f, L^+)$. And the line through $(f, L^-)$ with active coordinate set $I$ gives us $r + 1$ colour-focussed lines. Thus our induction is complete and the claim, and hence the result, follow.