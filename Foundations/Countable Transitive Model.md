For every finite $T\subseteq ZFC$ 
there is a countable [[Transitive Model]] $N$ of $T$.
### Proof
Consider the [[Von Neumann Hierarchy]] $\alpha \to V_{\alpha}$ with $V$ the set theoretic universe.
Let $T$ be finite and $\phi$ a formula equivalent to $T$ (just $\land$ all formulas)
Then $\phi$ is true as $T\subseteq ZFC$.
Thus find $\nu$ such that $V_{\nu}$ where $\phi$ is [[Absolute]] using [[Lévy Reflection Theorem]].
In particular $V_{\nu}\models \phi$
But then $V_{\nu}$ is a [[Transitive Model]] of $T$ as each $V_{\alpha}$ is a [[Foundations/Set Theory/Transitive|Transitive]] set.

Now apply [[The Downward Löwenheim-Skolem Theorem]] 
to construct a countable [[Substructure]] $M$ of $V_{\nu}$ 
such that all formulas in $T$ are [[Absolute]] between $M$ and $V_{\nu}$.
In particular $M\models T$.

Take countable $M$ from above.
Note that $\in$ is [[Well-Founded]] in $M$ (since [[Axiom of Foundation]] is true)
WLOG assume that [[Axiom of Extensionality]] is in $T$.
By [[Mostowski's Collapsing Theorem]] there is some $(N,\in)\cong(M,\in)$
where $N$ is [[Foundations/Set Theory/Transitive|Transitive]].
and since $M$ is countable, so is $N$ and $N\models T$

### Remark
When we defined $M$ above, it wasn't necessarily [[Foundations/Set Theory/Transitive|Transitive]] 
(so we needed the last step)
Let $\phi(x)$ be the statement "$x$ is the smallest uncountable [[Ordinal]]"
Then $V_{\nu}\models \phi(\aleph_{1})$
To see this note:
Being an [[Ordinal]] is [[Absolute]], so $\aleph_{1}$ is an ordinal in $V_{\nu}$
Countability is $\Sigma_{1}$ so [[Upwards Absolute]] so 
$$
V_{\nu} \models \aleph_{1} \text{ is uncountable}
$$
If $\alpha<\aleph_{1}$, its countability is witnessed by $f:\omega \to \alpha$ surjective.
But then $f\in V_{\alpha+2}\subseteq V_{\nu}$ so $V_{\nu}\models \alpha\text{ is countable}$

In particular, we have $V_{\nu}\models \exists x\,\phi(x)$.
Let $\Phi$ the set of all subformulas of $\exists x\,\phi(x)$.
Now $w(\phi,\varnothing)\in M$ by construction, but $\aleph_{1}$ is the only witness to $\exists x\,\phi(x)$
so $\aleph_{1}\in M$.
But $\aleph_{1}\not\subseteq M$ as $M$ is countable,
so $M$ is not [[Foundations/Set Theory/Transitive|Transitive]].
### Corollary
"Being countable" and "being cardinal"
are not [[Absolute]] statements between $N$ and $V_{\nu}$.
In particular, countable is $\Sigma_{1}$ 
and cardinal is $\Pi_{1}$
#### Proof
Suppose $\exists x\,\phi(x)$ from above is in $T$
where $\phi(x)$ means "$x$ is the smallest uncountable ordinal"
Then:
$$
V_{\nu}\models \exists x\,\phi(x)
$$
therefore
$$
N\models \exists x\, \phi(x)
$$
But any $\alpha \in N$ that is a witness:
$$
N\models \phi(\alpha)
$$
necessarily has to be $\alpha \subseteq N$ as $N$ is [[Foundations/Set Theory/Transitive|Transitive]]
Then $\alpha$ is countable and 

