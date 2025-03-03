The language has no operation symbols $\Omega=\emptyset$ and one binary predicate $\in$
There will be 9 sentences of the theory (axioms)
A model of ZF we denote by $V$ 
So $V$ is a non-empty set with an interpretation of $\in$ as a subset $\in_{V}$ of $V\times V$ 
Elements of $V$ will be called 'sets'
If $(a,b)$ is in $\in_{V}$ then say '$a$ is a member of $b$' or '$a$ belongs to $b$'
$V$ will be called the 'universe of sets'
## Axioms of ZF
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
