We have seen that $p:\tilde{X}\to X$ is a path connected covering space
$x_{0}\in X$ and $\tilde{x}_{0}\in p ^{-1}(x_{0})$ the map $p_{*}:\pi_{1}(\tilde{X},\tilde{x}_{0})\to \pi_{1}(X,x_{0})$ is injective

So $p_{*}\pi_{1}(\tilde{X},\tilde{x}_{0})\leq \pi_{1}(X,x_{0})$ a subgroup

If $\tilde{x}_{0}'\in p ^{-1}(x_{0})$ is another basepoint of $\tilde{X}$, 
as $\tilde{X}$ path-connected, can choose a path $\gamma:\tilde{x}_{0}\leadsto \tilde{x}_{0}'$.
Then $p\circ \gamma$ is a loop in $X$ based at $x_{0}$, $[p\circ \gamma]\in \pi_{1}(X,x_{0})$
and 
$[p\circ \gamma]^{-1}\cdot p_{*}\pi_{1}(\tilde{X},\tilde{x}_{0})\cdot[p\circ \gamma]=p_{*}\pi_{1}(\tilde{X},\tilde{x}_{0}')\leq \pi_{1}(X,x_{0})$
ie the two subgroups obtained are conjugate.

So fixing $(X,x_{0})$ we have functions
$$
\{ \text{based covering maps }p:(\tilde{X},\tilde{x}_{0})\to(X,x_{0}) \}\to \{ \text{subgroups of }\pi_{1}(X,x_{0}) \}
$$
and 
$$
\left\{  \text{covering map }p:\tilde{X}\to X  \right\}\to \{ \text{conjugacy classes of subgroups of } \pi_{1}(X,x_{0})\}
$$
Want to show that imposing appropriate equivalence relations of LHSs, makes those into bijections.

### Proposition
Suppose that $X$ is path-connected, [[Locally Path Connected]], and [[Semi-locally Simply Connected]].
Then for any subgroup $H\leq \pi_{1}(X,x_{0})$ there is a covering space $p:(\tilde{X},x_{0})\to(X,x_{0})$ with $p_{*}\pi_{1}(\tilde{X},\tilde{x}_{0})=H$
#### Proof
Let $q:\bar{X}\to X$ be the [[Universal Cover]] that we constructed, whose underlying set is the set of homotopy classes of paths in $X$ starting at $x_{0}$.
Define $\sim_{H}$ on $\bar{X}$ by $[\gamma]\sim_{H}[\gamma']$ iff $\gamma(1)=\gamma'(1)$ and $[\gamma \cdot(\gamma')^{-1}]\in H\leq \pi_{1}(X,x_{0})$
This is an equivalence relation
1. $[\gamma]\sim_{H}[\gamma]$ as $[c_{x_{0}}]\in H$ ($H$ contains the identity element)
2. $[\gamma]\sim_{H}[\gamma']$ then $[\gamma \cdot(\gamma')^{-1}]\in H$ so its inverse $[\gamma'\cdot \gamma ^{-1}]\in H$
3. $[\gamma]\sim_{H}[\gamma']\sim_{H}[\gamma'']$ then $[\gamma \cdot(\gamma')^{-1}]\in H$ and $[\gamma'\cdot(\gamma'')^{-1}]\in H$ so the product $[\gamma \cdot(\gamma'')^{-1}]\in H$.
So $\sim_{H}$ is an equivalence relation on $\bar{X}$

Define $\tilde{X}_{H}=\bar{X} / \sim_{H}$
and $p_{H}:\tilde{X}_{H}\to X$ to be the induced map $[[\gamma]]\to \gamma(1)$
