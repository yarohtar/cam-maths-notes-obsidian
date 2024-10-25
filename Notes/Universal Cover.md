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
Given a $y\in U$ pick a path $\gamma:x\leadsto y$ in $U$.
Then the following commutes:

```tikz
\usepackage{tikz-cd}

\begin{document}
\begin{tikzcd}
\pi_1(U,x) \arrow[r,"0"] \arrow[d,"Y_{\#}"] & \pi_1(X,x)\arrow[d,"Y_{\#}"]\\
\pi_1(U,y)\arrow[r] & \pi_1(X,y)
\end{tikzcd}
\end{document}
```

##### Step 1
Topology on $\tilde{X}$. For $[\alpha]\in \tilde{X}$, and $U\in \mathcal{U}$, define:
$$
([\alpha],U)=\{ [\beta]\in \tilde{X}:[\beta]=[\alpha \cdot \alpha'], \text{some path in }U\text{ starting at }\alpha(1) \}
$$
Let $\tilde{U}$ be the sellection of all these.
##### Claim 1
$\tilde{U}$ is a basis for a topology on $\tilde{X}$ (which we'll then use)
###### Proof
Assume $[\beta]\in([\alpha_{0}],U_{0})\cap([\alpha_{1}],U_{1})$ where $([\alpha_{i}],U_{i})\in \tilde{U}$
Need: $([\alpha_{2}],U_{2})\in \tilde{U}$ st $[\beta]\in([\alpha_{2}],U_{2})\subseteq([\alpha_{0}],U_{0})\cap([\alpha_{1}],U_{1})$
Fix $W\in \mathcal{U}$ st $\beta(1)\in W$ and $W\in U_{0}\cap U_{1}$
Now choosing $\alpha_{2}=\beta$ and $U_{2}=W$ for above works.
##### Step 2
Check this topology has the desired properties.
1. $p:\tilde{X}\to X$ with $[\gamma]\to \gamma(1)$ is cts
###### Proof
Suppose $U\in \mathcal{U}$, $[\alpha]\in p ^{-1}(U)$. Then $([\alpha],U)\subseteq p ^{-1}(U)$ and $([\alpha],U)\in \tilde{U}$ so $p ^{-1}(U)$ open.
2. $p$ is a covering map?
###### Proo