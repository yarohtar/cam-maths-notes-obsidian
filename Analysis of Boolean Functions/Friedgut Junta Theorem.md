Let $f:\{ -1,1 \}^{n}\to \{ -1,1 \}$ be a function on the $p$-[[Biased Cube]].
Suppose that 
$$
\lVert f^{(\leq k)} \rVert _{2}^{2} \geq 1-\epsilon
$$
Then there exists an $m$-[[Junta]] $g:\{ -1,1 \}^{n}\to \mathbb{R}$ with
$$
\lVert g-f \rVert _{2}^{2}\leq 2\epsilon
$$
and $m\leq\dots$
#### Proof
Let $\tau>0$ (to be chosen later)
and let 
$$
J=\{ i:\mathrm{Inf}_{i}f\geq \tau \}
$$
Let $\rho=\frac{\sigma^{2}}{4}$
Now note
$$
\sum_{i\not\in J}\mathrm{Stab}_{\rho}(D_{i}f)\leq \sum_{i\not\in J}\lVert D_{i}f \rVert _{\frac{4}{3}}^{2} = \sum_{i\not\in J}\lVert D_{i}f \rVert _{2}^{3} \sigma^{-1}
$$
by the [[Bonami Lemma]] and the fact that $D_{i}f\in \{ -\sigma,0,\sigma \}$ 

