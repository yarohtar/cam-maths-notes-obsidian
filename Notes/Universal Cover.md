A [[Covering Spaces|covering]] map $p:\tilde{X}\to X$ is a universal cover if $\tilde{X}$ is [[Simply connected]].


### Theorem
Let $X$ be path connected (1), [[Locally Path Connected]] (2), and [[Semi-locally Simply Connected]] (3). Then there exists a covering $p:\tilde{X}\to X$ with $\tilde{X}$ simply connected.

A NONEXAMINABLE PROOF
#### Proof
Fix $x_{0}\in X$.
Define aas a set:
$$
\tilde{X}=\{ \text{paths in } X \text{ starting at }x_{0} \text{ and ending anywhere up to htpy of paths} \}
$$
$p:\tilde{X}\to X$ with $[\gamma]\to \gamma(1)$
Need topology on $\tilde{X}$ st 
1. $p$ cts
2. $p$ covering map
3. $\tilde{X}$ simply connected
##### Step 0
Topology on $X$, revisited.
$$\mathcal{U}=\{ U\in X: U \text{ open in } X \text{ and } U \text{ path-connected and } \pi_{1}(U,x)\to \pi_{1}(X,x) \text{trivial for all }x\}$$

##### Claim 0
$\mathcal{U}$ basis for rthe topology on $X$
###### Proof
Assume $V\subseteq X$ open and $x\in V$. Need $U\in \mathcal{U}$ st $x\in U\subseteq V$
- $X$ is semilocally simply connected so there is some $U'$ open with $x\in U'$ st $\pi_{1}(U',x)\to \pi_{1}(X,x)$ trivial
- $X$ locally path-connected $\implies$ there is some $U$ open, path-connected st $x\in U\subseteq U'\cap V$
- Have $U\subseteq U'\subseteq X$ inducing 
$$
\pi_{1}(U,x)\to \pi_{1}(U',x)\to \pi_{1}(X,x)
$$
Second map has image 0, so composition has to be trivial.
Still need: $\pi_{1}(U,y)\to \pi_{1}(X,y)$ trivial for all $y\in U$.