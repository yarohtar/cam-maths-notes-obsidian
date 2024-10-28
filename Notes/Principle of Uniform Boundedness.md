$X$ [[Banach Space]], $Y$ [[Normed Spaces]].
$T_{1},T_{2},\dots \in L(X,Y)$. Suppose that $T_{n}$ are pointwise bounded.
Then the $T_{n}$ are uniformly bounded.
#### Proof
For $n=1,2,\dots$ let $E_{n}=\{ x\in X:\forall i\lVert T_{i}(x) \rVert\leq n \}$
Then each $E_{n}$ is closed (intersection of closed sets)
And $\bigcup E_{n}=X$ (by pointwise boundedness)
So by [[The Baire Category Theorem]] we have $B(X,\epsilon)\subseteq E_{n}$ for some $n$, some $x\in X$, some $\epsilon>0$.
So for any $y\in X$, $\lVert y \rVert<\epsilon$
