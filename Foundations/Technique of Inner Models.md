We prove that if $M\models ZFC$ then there is a [[Transitive Model]] $N\subseteq M$
such that 
$$
N\models ZFC+CH
$$
where $CH$ is [[The Continuum Hypothesis]]:
$$
2^{\aleph_{0}}=\aleph_{1}
$$
[[Sufficiently Strong]]
[[Absoluteness of Truth in a Model]]

### Proof
Fix set $X$, formula $\phi$, $p \in X^{<\omega}$.
Define
$$
\mathcal{D}(\phi,p,X) = \{ z\in X : X\models \phi(p,z) \}
$$
This is the subset of $X$, defined by $\phi$, with parameters $p$.
Define further
$$
\mathcal{D}(X) = \{ \mathcal{D}(\phi,p,X) :  \}
$$