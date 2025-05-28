[[Axiom of Extensionality]]
[[Axiom of Separation]]
[[Empty-set axiom]]
[[Pair-set axiom]]
[[Union axiom]]
[[Power-set axiom]]
[[Axiom of Infinity]]
So far we can do quite a bit of mathematics with our axioms, and also any model $V$ is infinite. 
[[Successor]]
But we do not yet have infinite sets (because $V$ is not a set)
The axiom of infinity asserts the existence of a [[Successor Set]]
$$
(\exists x)(x\text{ is a successor set})
$$

We can then show that there's a smallest successor set, i.e. we can prove 
$$
(\exists x)(x\text{ is a successor set}\land(\forall y)(y\text{ is a successor set})\implies x\subseteq y)
$$
To prove it,
In a model, pick a successor set $y$ using (Inf). Form the set
$$
z=\{ t\in \mathbb{P}y\mid t \text{ is a successor set} \}
$$
Since $y\in z$ we can form $x=\bigcap z$. It's easy to check that $x$ is the smallest successor set, which we denote by $\omega$.

Every successor set contained in $\omega$ is $\omega$ i.e.
$$
(\forall x\subseteq \omega)((0\in x\land(\forall y\in x)(y^{+}\in x))\implies x=\omega)
$$
where $(\forall a\subseteq b)p$ is a shorthand for $(\forall a)(a\subseteq b\implies p)$
for any formula $p$ 

So inside $V$ we have true induction! We call this $\omega$-induction
But still, from the outside there may be subsets of $\omega$ that are not sets in $V$ 

### Axiom of Replacement (Rep)
[[Class]]
The Axiom of Replacement is the axiom-scheme asserting that the image of a set under a [[Function Class]] is a set. As usual, we'll have parameters:
$$
\begin{gather}
(\forall t_{1})\dots(\forall t_{n})(\\
(\forall x)(\forall y)(\forall z)((p\land p[z/ y])\implies y=z)\\
\implies(\forall x)(\exists y)(\forall z)(z\in y\iff(\exists u)(u\in x\land p[u/ x, z / y]))
)
\end{gather}
$$
### Axiom of Foundation (Fnd)
$$
(\forall x)(\neg(x=\emptyset)\implies(\exists y)(y\in x\land (\forall z\in x)\neg(z\in y)))
$$

## 
The 9 axioms and axiom schemes form ZF set theory.
The [[Axiom of Choice]] is not included. We write ZFC for ZF+AC