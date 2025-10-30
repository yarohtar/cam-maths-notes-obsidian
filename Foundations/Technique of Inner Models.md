We prove that if $M\models ZFC$ then there is a [[Transitive Model]] $N\subseteq M$
such that 
$$
N\models ZFC+CH
$$
where $CH$ is [[The Continuum Hypothesis]]:
$$
2^{\aleph_{0}}=\aleph_{1}
$$
[[Sufficiently Strong]]
[[Absoluteness of Truth in a Model]]

### Proof
Let $L$ be the [[Constructible Hierarchy]].
We want to prove that
$$
L\models ZF(C)
$$
Any [[Transitive Model]] satisfies [[Axiom of Extensionality]] and [[Axiom of Foundation]].
Also $X=\omega$ is [[Absolute]], and $\omega$ satisfies [[Axiom of Infinity]],
we also get $L_{\alpha}\models$[[Axiom of Infinity]] for all $\alpha>\omega$.
The operations $x,y\to \{ x,y \}$ and $x\to \bigcup x$ are [[Absolute Operation]]
for a [[Sufficiently Strong]] $T$.
So we only need to prove
$$
(\forall x,y\in L) \left( \{ x,y \}\in L \land \bigcup x\in L \right)
$$
Find $\{ x,y \}$ in $L$.
Assume $x,y\in L$.
Take some $\alpha$ such that $x,y\in L_{\alpha}$.
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
The union is exactly the same.
Now we consider the [[Power-set axiom]]
This is more complicated, because it is not [[Absolute]]. 
(But if it was absolute, it would be hopeless to find a powerset in a countable model)
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

Now consider [[Axiom of Separation]].
We need the set
$$
\{ z\in x: L\models \phi(z,p) \}
$$
where $p$ are parameters.
Take formula 
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
Apply [[Lévy Reflection Theorem]] to find $\alpha$ 
such that $\phi$ is [[Absolute]] between $L_{\alpha}$ and $L$.
Thus
$$
D(\psi,(x,p),L_{\alpha}) = \{ z\in x:L\models \phi(z,p) \}
$$
and so separation holds.

[[Axiom of Replacement]] is on Example Sheet 2.

The only one left is the [[Axiom of Choice]]
We can provide a [[Well-ordered|well-order]] of $L$:
Fix some some $<_{\omega}$ on $L_{\omega}$ of [[Order Type]] $\omega$.
Assume that $<_{\alpha}$ is a wellorder of $L_{\alpha}$,
define lexifcographically a wellorder of 
$$
\mathrm{Fml}\times L_{\alpha}
$$
and then write for $x\in L_{\alpha+1}$ 
$$
w(x) = \mathrm{min}_{<_{\alpha}} \{ (\phi,) \}
$$
