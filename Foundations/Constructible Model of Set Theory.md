The [[Constructible Hierarchy]] $L$ satisfies:
$$
L\models ZF
$$
### Proof
We examine the [[Axioms of ZF]] individually.
#### Structural axioms
Any [[Transitive Model]] satisfies [[Axiom of Extensionality]] and [[Axiom of Foundation]].
Also $x=\omega$ is [[Absolute]], and $\omega$ satisfies [[Axiom of Infinity]],
we also get $L_{\alpha}\models$[[Axiom of Infinity]] for all $\alpha>\omega$.
#### Functional Axioms
##### Pair and Union
The operations $x,y\to \{ x,y \}$ and $x\to \bigcup x$ are [[Absolute Operation]]s
for a [[Sufficiently Strong]] $T$.
So we only need to prove
$$
(\forall x,y\in L) \left( \{ x,y \}\in L \land \bigcup x\in L \right)
$$
Assuming $x,y\in L$, take some $\alpha$ such that $x,y\in L_{\alpha}$.
Consider:
$$
\phi(z,x,y) = (z=x)\lor(z=y)
$$
Form
$$
\begin{align}
D(\phi,(x,y),L_{\alpha})  & = \{ z\in L_{\alpha} : L_{\alpha}\models \phi(z,x,y) \} \\
 & =\{ z\in L_{\alpha} : L_{\alpha}\models z=x \lor z=y \} \\
 & =\{ z\in L_{\alpha} : z=x \lor z=y \}  \\
 & = \{ x,y \}
\end{align}
$$
The union is essentially the same.
##### Powerset
This is more complicated, because [[Powerset Axiom]] is not [[Absolute]]. 
(But if it was [[Absolute]], it would be hopeless to find a powerset in a countable model)
Note that $z\subseteq x$ is [[Absolute]].
Thus if $p$ is a powerset of $x$ then $p\subseteq \mathcal{P}x$.
Also clearly $p\subseteq L$ as $L$ is [[Foundations/Set Theory/Transitive|Transitive]].
Thus our candidate is $p=\mathcal{P}x\cap L$.
If $p \in L$ then $p$ satisfies the conditions of the powerset axiom.
Define 
$$
\Omega=\{ \rho_{L}(z) : z\subseteq x, z\in L \}
$$
By [[Axiom of Replacement]] this is a set, 
and it is a set of ordinals, so it has to have an upper bound
so there is some $\vartheta$ such that $\Omega \subseteq \vartheta$,
so $p\cap L\subseteq L_{\vartheta}$.
Let
$$
\phi(z,x) = z\subseteq x
$$
then $p=D(\phi,x,L_{\vartheta})$ and thus $p \in L_{\vartheta+1}\subseteq L$.

##### Separation
[[Axiom of Separation]]
For any formula $\phi$, we need the set
$$
\{ z\in x: L\models \phi(z,p) \}
$$
where $p$ are parameters.
Take the formula 
$$
\psi(z,x,p) = z\in x\land \phi(z,p)
$$
Then
$$
\begin{align}
D(\psi,(x,p),L_{\alpha})  & = \{ z\in L_{\alpha} : L_{\alpha}\models z\in x \land \phi(z,p) \} \\
 & =\{ z\in x: L_{\alpha}\models \phi(z,p) \}
\end{align}
$$
This only works if $\phi$ is [[Absolute]] between $L_{\alpha}$ and $L$.
Apply [[Lévy Reflection Theorem]] to find such $\alpha$.
Thus
$$
D(\psi,(x,p),L_{\alpha}) = \{ z\in x:L\models \phi(z,p) \}
$$
and so separation holds.
##### Replacement
[[Axiom of Replacement]] is on Example Sheet 2.
