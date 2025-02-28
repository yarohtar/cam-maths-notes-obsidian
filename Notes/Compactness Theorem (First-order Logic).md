Let $S$ be a first-order theory.
If every finite subset of $S$ has a model, then $S$ has a model.

#### Proof
If $S\models \bot$ then $S\vdash \bot$ by [[Adequacy Theorem (First-order Logic)]]
As proofs are finite, there's a finite $S'\subseteq S$ s.t. $S'\vdash \bot$. Then by the [[Soundness Theorem (First-order Logic)]] $S'\models \bot$ i.e. $S'$ has no model.