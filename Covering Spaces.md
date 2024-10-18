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
Let $y\in Y\setminus S$ ie $\tilde{f}_{0}(y)\neq \tilde{f}_{1}(y)$.
Let $f(y)\in U$
$p ^{-1}(U)=\sqcup_{\alpha \in I} V_{\alpha}$ as before

Have $\tilde{f}_{0}(y)\in V_{\beta}$, $\tilde{f}_{1}(y)\in V_{\gamma}$
$N=\tilde{f}_{0}^{-1}(v_{\beta})\cap \tilde{f}_{1}^{-1}(V_{\gamma})$ open in $Y$.
As $p|_{V_{\beta}}$ and $p|_{V_{\gamma}}$ are homeomorphisms, get $N\subseteq Y\setminus S$ so $Y\setminus S$ is open


### Homotopy lifting lemma
Let $p:\tilde{X}\to X$ be a covering map, $H:Y\times I\to X$ a homotopy from $f_{0}$ to $f_{1}$, $\tilde{f}_{0}$ a lift of $f_{0}$. Then there exists a unique homotopy $\tilde{H}:Y\times I\to \tilde{X}$ such that 
1. $\tilde{H}(\cdot,0)=\tilde{f}_{0}(\cdot)$
2. $p\circ \tilde{H}=H$
#### Proof
Let $\{ U_{\alpha} \}_{\alpha \in I}$ open cover of $X$ by evenly covered sets.
Say $p ^{-1}(U)=\sqcup_{\beta \in I_{\alpha}}V_{\beta}$, $p|_{V_{\beta}}:v_{\beta}\to U_{\alpha}$
$\cup_{\alpha}H^{-1}(U_{\alpha})$ cover $Y\times I$
By [[Lebesgue number lemma]] there is some $N$ and $W_{y_{0}}$ an open nbd of $y_{0}$ in $Y$ such that 
for all $i=0,\dots N-1$ there is some $\alpha \in I$ such that 
$W_{y_{0}}\times\left[ \frac{1}{N}, \frac{i+1}{N} \right]$