Let $G$ be a [[Function Class]] defined everywhere.
Then there is a function class $F$ defined everywhere
such that:
$$
(\forall x)(F(x)=G(F|_{x}))
$$
Also $F$ is unique.
Note $F|_{x}$ is the set $\{ (s,F(s)) : s \in x \}$
which is a set by [[Axiom of Replacement]]
### Proof
Uniqueness by [[Principle of Epsilon-Induction]]

We say $f$ is an attempt if
- $f$ is a function
- $\operatorname{dom}f$ is transitive
and 
$$
(\forall x)(x\in \operatorname{dom}f \implies f(x)=G())
$$