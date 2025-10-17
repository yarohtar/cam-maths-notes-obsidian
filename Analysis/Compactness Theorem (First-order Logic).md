Let $S$ be a first-order [[Theory]].
If every finite subset of $S$ has a model, then $S$ has a model.

#### Proof
If $S\models \bot$ then $S\vdash \bot$ by [[Adequacy Theorem (First-order Logic)]]
As proofs are finite, there's a finite $S'\subseteq S$ s.t. $S'\vdash \bot$. Then by the [[Soundness Theorem (First-order Logic)]] $S'\models \bot$ i.e. $S'$ has no model.

### Corollary 
Finite groups cannot be axiomatized as a first-order theory.
#### Proof
Suppose $T$ is a theory in some language $L$ whose models are exactly the finite groups. Then let
$S=T\cup \{ \neg t_{1},\neg t_{2},\dots \}$
where 
$t_{n}=(\exists x_{1})\dots(\exists x_{n})(\forall x)(x=x_{1}\lor\dots \lor x=x_{n})$
Any finite subset of $S$ has a model, eg the cyclic $C_{n}$ for $n$ sufficiently large
By [[Compact]] $S$ has a model.

### Corollary
If a first order theory $T$ has arbitrarily large finite models, then it has an infinite model.
#### Proof
Essentially the same.
### Corollary
[[The Upwards Löwenheim-Skolem Theorem]]
