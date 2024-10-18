A covering space of a space $X$ is a pair $(\tilde{X}, p)$ where
- $\tilde{X}$ is a space
- $p: \tilde{X}\to X$ is a map such that for all $x \in X$ there is a [[Neighbourhood|nbd]] $U$ of $x$ such that $p ^{-1}(U)=\sqcup_{\alpha\in A}V_{\alpha}$, where $V_{\alpha}\subset \tilde X$ open, $p|_{V_{\alpha}}:V_{\alpha}\to U$ is a homeomorphism
$p$ is called a covering map. Open sets $U$ as above are called evenly covered.
### Definition
Let $p: \tilde{X}\to X$ covering space, $f:Y\to X$
A lift of $f$ along $p$ is a map $\tilde{f}:Y\to \tilde{X}$ such that the whole thing commutes ie $p\circ \tilde{f}=f$.

### Lemma
Let $p: \tilde{X}\to X$ covering map, and $f:Y\to X$ map. Let $\tilde{f}_{0},\tilde{f}_{1}:Y\to \tilde{X}$ tow lifts of $f$. Then
$S=\{ y \in Y\mid \tilde{f}_{0}(y)=\tilde{f_{1}}(y) \}$ is open and closed in $Y$.
#### Proof
##### $S$ open
Fix $y \in S$. Let $f(y)\in U$ evenly covered nbd in $X$. 
Say $p ^{-1}(U)=\sqcup_{\alpha \in I} V_{\alpha}$
Have $\tilde{f}_{0}(y)=\tilde{f}_{1}(y)\in V_{\beta}$, $\beta \in I$.
Set $N=\tilde{f}^{-1}_{0}(V_{\beta})\cap \tilde{f}^{-1}_{1}(V_{\beta})$ (open in $Y$)
As $p|_{V_{\beta}}$ is a homeomorphism, get $\tilde{f}_{0}|_{N}=\tilde{f}_{1}|_{N}$ so $S$ is open.

##### $S$ closed
Let $y\in Y-S$ ie $\tilde{f}_{0}(y)\neq \tilde{f}_{1}(y)$.
Let $f$