A covering space of a space $X$ is a pair $(\tilde{X}, p)$ where
- $\tilde{X}$ is a space
- $p: \tilde{X}\to X$ is a map such that for all $x \in X$ there is a [[Neighbourhood|nbd]] $U$ of $x$ such that $p ^{-1}(U)=\sqcup_{\alpha\in A}V_{\alpha}$, where $V_{\alpha}\subset \tilde X$ open, and $p|_{V_{\alpha}}:V_{\alpha}\to U$ is a [[Homeomorphism]]
$p$ is called a covering map. Open sets $U$ as above are called evenly covered.
### Definition (lift)
Let $p: \tilde{X}\to X$ be a covering map, and $f:Y\to X$ a map.
A lift of $f$ along $p$ is a map $\tilde{f}:Y\to \tilde{X}$ such that the whole thing commutes ie $p\circ \tilde{f}=f$.
[[Uniqueness of Lifts Lemma]]
[[Homotopy Lifting Lemma]]

### Definition (universal cover)
A covering map $p:\tilde{X}\to X$ is a universal cover if $\tilde{X}$ is [[Simply connected]].
### Definition ($n$ sheeted cover)
A covering map $p:\tilde{X}\to X$ is $n$ sheeted if each $p ^{-1}(x)$ has cardinality $n$ (where $n\in \mathbb{N}$ or $n=\infty$).