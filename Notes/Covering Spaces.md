A covering space of a space $X$ is a pair $(\tilde{X}, p)$ where
- $\tilde{X}$ is a space
- $p: \tilde{X}\to X$ is a map such that for all $x \in X$ there is a [[Neighbourhood|nbd]] $U$ of $x$ such that $p ^{-1}(U)=\sqcup_{\alpha\in A}V_{\alpha}$, where $V_{\alpha}\subset \tilde X$ open, and $p|_{V_{\alpha}}:V_{\alpha}\to U$ is a [[Homeomorphism]]
$p$ is called a covering map. Open sets $U$ as above are called evenly covered.
### Definition
Let $p: \tilde{X}\to X$ be a covering map, and $f:Y\to X$ a map.
A lift of $f$ along $p$ is a map $\tilde{f}:Y\to \tilde{X}$ such that the whole thing commutes ie $p\circ \tilde{f}=f$.

### Lemma
Let $p: \tilde{X}\to X$ be a covering map, and $f:Y\to X$ a map. Let $\tilde{f}_{0},\tilde{f}_{1}:Y\to \tilde{X}$ be two lifts of $f$. Then
$S=\{ y \in Y\mid \tilde{f}_{0}(y)=\tilde{f_{1}}(y) \}$ is open and closed in $Y$.
#### Proof
##### $S$ open
Fix $y \in S$. Let $f(y)\in U$ evenly covered nbd in $X$. 
Say $p ^{-1}(U)=\sqcup_{\alpha \in I} V_{\alpha}$
Have $\tilde{f}_{0}(y)=\tilde{f}_{1}(y)\in V_{\beta}$, $\beta \in I$.
Set $N=\tilde{f}^{-1}_{0}(V_{\beta})\cap \tilde{f}^{-1}_{1}(V_{\beta})$ (open in $Y$)
As $p|_{V_{\beta}}$ is a homeomorphism, get $\tilde{f}_{0}(n)=\tilde{f}_{1}(n)=p|_{V_{\beta}} ^{-1}(f(n))$ for all $n\in N$ so $\tilde{f}_{0}|_{N}=\tilde{f}_{1}|_{N}$ so $S$ is open.

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
Let $\{ U_{\alpha} \}_{\alpha \in I}$ be an open cover of $X$ by evenly covered sets.
Say $p ^{-1}(U_{\alpha})=\sqcup_{\beta \in I_{\alpha}}V_{\beta}$, with $p|_{V_{\beta}}:V_{\beta}\to U_{\alpha}$ a homeomorphism 
$$
\bigcup_{\alpha}H^{-1}(U_{\alpha})\quad\text{ cover } \quad Y\times I
$$

Fix $y_{0}\in Y$.
By [[Lebesgue number lemma]] applied to $\{ y_{0} \}\times I$, there is some $N$ st $\{ y_{0} \}\times\left[ \frac{i}{N}, \frac{i+1}{N} \right]\subseteq H^{-1}(U_{\alpha(i)})$ for some $\alpha(i)$.
Furthermore, due to compactness of $\left[ \frac{i}{N}, \frac{i+1}{N} \right]$ we know that there is some open $W_{y_{0}}'$ (a nbd of $y_{0}$), such that $H\left( W_{y_{0}}^{(i)}\times\left[ \frac{i}{N}, \frac{i+1}{N} \right] \right)\subseteq U_{\alpha(i)}$. 
(Idea is find the open neighbourhoods of $H(y_{0},r)$ for each $r$ and then take their inverses, convert those into $Y_{k}\times V_{k}$, then find the finite cover of the interval by $V_{k}$$s$ and then intersect $Y_{k}$$s$ to obtain an open nbd of $y_{0}$)

##### Step 1
Find $\beta \in I_{\alpha(0)}$ such that $\tilde{f}_{0}(y_{0})\in V_{\beta}$. Find an open nbd of $\tilde{f}_{0}(y_{0})$ in $V_{\beta}$ and intersect it with $W_{y_{0}}^{(i)}$ to obtain $W_{y_{0}}$.
Now $\tilde{f}_{0}(W_{y_{0}})\subseteq V_{\beta}$ 


Now find $W_{y_{0}}'$ an open nbd of $y_{0}$ in $Y$ such that $W_{y_{0}}'\times\left[ 0, \frac{1}{N} \right]\subseteq H^{-1}(U_{\alpha})$.
and $W_{y_{0}}'$ an open nbd of $y_{0}$ in $Y$ such that 
for all $i=0,\dots N-1$ there is some $\alpha \in I$ such that 
$W_{y_{0}}'\times\left[ \frac{i}{N}, \frac{i+1}{N} \right]\subseteq H^{-1}(U_\alpha)$.
Additionally, pick $\beta$ st $y_{0}\in V_{\beta}$ and set $W_{y_{0}}=W_{y_{0}}'\cap \tilde{f}_{0}^{-1}(V_{\beta})$ 
Now construct lift $\tilde{H}|_{W_{y_{0}}\times I}$ of $H|_{W_{y_{0}}\times I}$.
Firstly, $\tilde{f}_{0}$ maps $W_{y_{0}}$ to some $V_{\beta}$ 
Set
$$
\tilde{H}|_{W_{y_{0}}\times\left[ 0, \frac{1}{N} \right]}=(p|_{V_{\beta}})^{-1}\circ H|_{W_{y_{0}}\times\left[ 0, \frac{1}{N} \right]}:W_{y_{0}}\times\left[ 0, \frac{1}{N} \right]\to V_{\beta}
$$
##### Step 2
Proceed iteratively
Upshot:
Get map $\tilde{H}|_{W_{y_{0}}\times I}$ lifting $H|_{W_{y_{0}}\times I}$ and extending $\tilde{f}_{0}|_{W_{y_{0}}}$

##### Check
Lifts need to agree on $(W_{y_{0}}\times I)\cap(W_{y_{1}}\times I)=(W_{y_{0}}\cap W_{y_{1}})\times I$ ?
By previous lemma, they must agree on an open and closed subset of $(W_{y_{0}}\cap W_{y_{1}})\times I$.
By construction, they agree on $(W_{y_{0}}\cap W_{y_{1}})\times \{ 0 \}$
So they have to agree on all of $(W_{y_{0}}\cap W_{y_{1}})\times I$
eg by considering that they agree on $\{ y \}\times \{ 0 \}$ (for each $y\in W_{y_{0}}\cap W_{y_{1}}$) and $\{ y \}\times I$ are all connected.