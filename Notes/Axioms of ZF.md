### The Axiom of Extensionality (Ext)
If two sets have the same members then they are equal
$$
(\forall x)(\forall y)((\forall z)(z\in x \iff z\in y)\implies x=y)
$$
### Axiom of Separation (Sep)
Can take a subset of a set. This is an axiom scheme
$$
(\forall t_{1})\dots (\forall t_{n})(\forall x)(\exists y)(\forall z)(z\in y \iff(z\in x\land p))
$$
where $p$ is a formula with $FV(p)=\{ z,t_{1},\dots,t_{n} \}$
The set $y$ whose existence is asserted by (Sep) is unique by (Ext)
We denote this $y$ by $\{ z\in x\mid p \}$
Formally, we are introducing an $(n+1)$-arry operation symbol to the language.

### Empty-set axiom (Emp)
There is a set with no members
$$
(\exists x)(\forall y)\neg(y\in x)
$$
By (Ext) it is unique. We denote it by $\emptyset$

### Pair-set axiom (Pair)
For any sets $x$, $y$, can form $\{ x,y \}$
$$
(\forall x)(\forall y)(\exists z)(\forall t)(t\in z \iff(t=x\lor t=y))
$$
The unique (by (Ext)) is denoted by $\{ x,y \}$
We write $\{ x \}$ for $\{ x,x \}$
Formally, we introduced a binary symbol $\{ , \}$ and a unary symbol $\{  \}$
By (Ext) we haave $\{ x,y \}=\{ y,x \}$
We can now define [[Ordered Pair]] and [[Function]]

### Union axiom (Un)
Can form the union of a set
$$
(\forall x)(\exists y)(\forall z)(z\in y\iff(\exists t)(t\in x\land z\in t))
$$
The set $y$ whose existence is asserted here is unique by (Ext)
We denote this by $\bigcup x$ (formally, we are introducing a unary operation symbol $\bigcup$ to the language of ZF)
So $\bigcup x$ is the union of the members of $x$ 

We write $a \cup b$ for $\bigcup \{ a,b \}$

#### Intersection
We can prove 
$$
(\forall x)(\neg(x=\emptyset)\implies(\exists y)(\forall z)(z\in y\iff(\forall t)(t\in x \implies z\in t)))
$$
Indeed, start with a nonempty set $x$ and form the set
$$
y=\left\{  z\in \bigcup x\mid (\forall t)(t\in x \implies z\in t)  \right\}
$$
using (Un) and (Sep). Technically, we work in a model here and then we deduce the sentence above by [[Gödel's Completeness Theorem for First-Order Logic]]

The unique set $y$ constructed here is denoted by $\bigcap x$
We write $a\cap b$ for $\bigcap \{ a,b \}$

We can now define the domain of a [[Function]] $f$ 
If $(x,y)\in f$, then since $(x,y)=\{ \{ x \},\{ x,y \} \}$
we have $x,y\in \bigcup \bigcup f$
So we can form the set 
$$
dom\ f=\left\{  x\in \bigcup \bigcup f\mid (\exists y)((x,y)\in f)  \right\}
$$
using (Un) and (Sep)

Formally, we introduce a unary operation symbol $dom$
Note that this is defined for any set $f$ but it only has a meaning for functions.

### Power-set axiom (Pow)
We can form a power set of a set
$$
(\forall x)(\exists y)(\forall z)(z\in y\iff z\subseteq x)
$$
where $z\subseteq x$ is shorthand for $(\forall t)(t\in z\implies t\in x)$
The unique set $y$ is denoted by $\mathbb{P}x$
We can now construct the [[Cartesian Product]] of sets $x,y$

### Axiom of Infinity (Inf)
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