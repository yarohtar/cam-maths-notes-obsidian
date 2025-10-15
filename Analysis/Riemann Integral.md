Let $U\subseteq \mathbb{R}$ and $[a,b]\subseteq U$ (with $a\leq b$)
Let $f:U\to \mathbb{R}$ be a function.
Suppose $f$ is [[Riemann Integrable]] on $[a,b]$
with [[Upper Integral]] and [[Lower Integral]] equal to $I$ 
Then we say that the Riemann integral of $f$ is $I$ 
We write:
$$
\int_{a}^{b} f = I
$$
Additionally, define:
$$
\int_{b}^{a} f = -I
$$
If the domain $U$ contains $(N, \infty)$ for some $N$, 
define for all $a>N$:
$$
\int_{a}^{\infty} f = \lim_{x \to \infty} \int_{a}^{x} f
$$
$$
\int_{\infty}^{a} f = - \lim_{x \to \infty} \int _{a}^{x} f
$$
if the limit exists.
Similarly for $-\infty$.

If the domain $U=\mathbb{R}$, 
and both $\int_{0}^{\infty}f$ and $\int_{-\infty}^{0}f$ exist
then define:
$$
\int_{-\infty}^{\infty} f = \int_{-\infty}^{0}f + \int_{0}^{\infty} f
$$
