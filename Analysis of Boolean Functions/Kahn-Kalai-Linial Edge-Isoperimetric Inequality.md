Let $f:\{ -1,1 \}^{n}\to \{ -1,1 \}$ be a boolean function on the $p$-[[Biased Cube]].
Then there is some $i$ such that 
$$
\mathrm{Inf}_{i}f \geq \frac{9}{\tilde{I}(f)^{2}} \cdot 9^{-\tilde{I}(f)}
$$
where $\tilde{I}=\frac{I(f)}{\mathrm{Var}(f)}$ is the scaled total [[Influence]].
#### Proof
Let 
$$
S=\sum_{i=1}^{n} \mathrm{Stab}_{\frac{\sigma^{2}}{3}}(D_{i}f)
$$
Where $\mathrm{Stab}$ is [[Stability]].
It follows from [[Bonami Lemma]] that $\mathrm{Stab}_{\sigma^{2} / 3}(D_{i}f)\leq \lVert D_{i}f \rVert_{4 /3}^{2}$.
Then $D_{i}f(x)\in \{ -1,0,1 \}$ so $D_{i}f(x)^{4/3}=D_{i}f^{2}$ so
$$
\mathrm{Stab}_{\sigma^{2} / 3}(D_{i}f) \leq \lVert D_{i}f^{2} \rVert^{3 / 2} = (\mathrm{Inf}_{i}f)^{3/2}
$$
by definition of [[Influence]].
Let $i=\mathrm{argmax}_{j}\ \mathrm{Inf}_{j}f$ and conclude 
$$
S\leq (\mathrm{Inf}_{i}f)^{1/2} I(f)
$$
For the lower bound, use:
$$
\mathrm{Stab}_{\sigma^{2} /3}(D_{i}f) = \sum_{A\subseteq[n]} \left( \frac{\sigma^{2}}{3} \right)^{\lvert A \rvert } \widehat{D_{i}f}(A)
$$
and note 
$$
\widehat{D_{i}f}(A) = \begin{cases}
0 & i\not\in A \\

\end{cases}
$$
