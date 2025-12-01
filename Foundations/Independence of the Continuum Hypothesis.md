Let $M$ be a countable [[Transitive Model]] of $ZFC$.
Consider $\mathbb{P}=\mathrm{Fn}(\omega_{2}^{M}\times \omega, 2)$, the [[Finite Function Forcing]] (in $M$)
Let $G$ be a $\mathbb{P}$-[[Generic Filter]] over $M$ and 
$$
f=\bigcup G
$$
Then $f$ is a binary $\omega_{2}^{M}\times \omega$ matrix, and each row is a subset of $\omega$.
For $\alpha \neq \beta$ with $\alpha,\beta<\omega_{2}$ define 
$$
D_{\alpha,\beta} = \{ p\in \mathbb{P} : (\exists u)\, p(\alpha,u) \neq p(\beta,u) \}
$$
This is a set $D_{\alpha,\beta}\in M$ and it is [[Dense Below|Dense]] in $\mathbb{P}$.
Therefore 
$$
\hat{f}(\alpha) = \{ n : f(\alpha,n) = 1 \}
$$
is an injection from $\omega_{2}^{M}$ into $\mathcal{P}(\omega)$.
Thus we have proved that in the [[Model Extension by Finite Function Forcing]]: 
$$
M[G] \models 2^{\aleph_{0}} \geq \lvert \omega_{2}^{M} \rvert 
$$
We are not done yet!
We need $\omega_{2}^{M}=\omega_{2}^{M[G]}$ (which needs $\omega_{1}^{M}=\omega_{1}^{M[G]}$).
### Lemma
Given $M[G]$, there is no surjection:
$$
f:\mathbb{N}\to \omega_{1}^{M}
$$
#### Proof
Suppose there was. 
Clearly, $f\in M[G]\setminus M$.
Let $\tau$ be a [[Name]] for $f$: 
$$
M[G]\models \underbrace{\mathrm{val}(\tau,G) \text{ is a surjection } \mathbb{N}\to \omega_{1}^{M}}_{\varphi}
$$
By [[The Forcing Theorem]] find $p\in G$ such that $p\Vdash\varphi$.
For each $\alpha<\omega_{1}^{M}$ there is $n$ such that 
$$
M[G] \models f(n) =\alpha
$$
so there is some $q_{\alpha}\leq p$ such that 
$$
q_{\alpha} \Vdash \tau(\check{n}) = \check{\alpha}
$$
Fix $n\in \mathbb{N}$ and consider 
$$
F_{n} = \{ \alpha<\omega_{1}^{M} : (\exists q\leq p)\, q\Vdash \tau(\check{n})=\check{\alpha} \}
$$
Note that if $q\Vdash\tau(\check{n})=\check{\alpha}$ and $q\Vdash\tau(\check{n})=\check{\beta}$ then $\alpha=\beta$
Also $F_{n}\in M$ so 
$$
M\models \lvert F_{n} \rvert \leq \lvert \mathbb{P} \rvert 
$$
We conclude 
$$
\mathrm{ran}(f) \subseteq \bigcup_{n\in \mathbb{N}} F_{n}
$$
