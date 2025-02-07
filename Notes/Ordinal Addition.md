For [[Ordinal]]$s$ $\alpha$, $\beta$ we define $\alpha+\beta$ by recursion on $\beta$ with $\alpha$ fixed as follows:
$\alpha+0=\alpha$
$\alpha+\beta^{+}=(\alpha+\beta)^{+}$
$\alpha+\lambda=sup \{ \alpha+\beta:\beta<\lambda \}$ for $\lambda$ limit
#### Remark
Technically, we should fix an ordinal $\gamma$ and define $\alpha+\beta$ by recursion on $\beta$ in the [[Well-ordered]] set $I_{\gamma}$. By uniqueness in recursion, this gives a well-defined $\alpha+\beta$ for all $\alpha,\beta$. In general, this justifies recursive definition on all ordinals like the one above.

Similarly, proof by induction on all ordinals works;
Let $p(\alpha)$ be some property of an ordinal $\alpha$. Then
$$
(\forall \alpha)((\forall \beta)((\beta<\alpha)\implies p(\beta))\implies p(\alpha))\implies(\forall \alpha)p(\alpha)
$$
Indeed, assume otherwise. Then there is an ordinal $\gamma$ such that $\neg p(\gamma)$. Then there is also a least ordinal $\alpha\leq \gamma$ such that $\neg p(\alpha)$. If $$