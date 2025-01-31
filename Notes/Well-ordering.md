A well-ordering of a set $X$ is a [[Linear order]] $<$ on $X$ s.t. every nonempty subset of $X$ has a least element:
$$
(\forall S\subseteq X)(S\neq \emptyset \implies(\exists x\in S)(\forall y\in S)(x\leq y))
$$
This least element is unique by antisymmetry of $\leq$

This property is preserved by [[Order-isomorphism]].

### Lemma
Let $X$, $Y$ be well-ordered sets, $I$ be an [[Initial Segment]] of $Y$ and $f:X\to I$ be an [[Order-isomorphism]]. Then for every $x\in X$, we have 
$$
f(x)=min(Y\setminus \{ f(y):y<x \})
$$
