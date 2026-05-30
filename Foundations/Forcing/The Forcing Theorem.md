Let $M$ be a countable [[Transitive Model]] and $\mathbb{P}\in M$ a [[Forcing Partial Order]].
Then there is an [[Absolute]] [[Forcing Relation]] $\Vdash$ on $\mathbb{P}\times \mathrm{Se nt}_{\mathbb{P},M}$.
## Proof (chunky one)
### Definition of $\Vdash$
We first define the [[Forcing Relation]] $\Vdash$ on atomic formulas.
From the definition of the [[Forcing Relation]], 
we want $\sigma^{G}\in \tau^{G}$ precisely when some $p\in G$ has $p\Vdash \sigma \in \tau$.
Note that $\sigma^{G}\in \tau^{G}$ iff $(\pi,s)\in \tau$ and $\sigma^{G}=\pi^{G}$ for some $s\in G$.
But then also $\sigma^{G}=\pi^{G}$ iff some $q\in G$ has $q\Vdash \sigma=\pi$.

We conclude that $p\Vdash \sigma \in \tau$ iff any filter $G$ containing $p$
has some $(\pi,s)\in \tau$ with $s \in G$ and $q\in G$ with $q\Vdash \sigma=\pi$.
It is then convenient to look at 
$$
D(\tau)=\{ q\leq p: (\exists(\pi,s)\in \tau)\ q\leq s\land q\Vdash \sigma=\pi \}
$$
If this set is [[Dense Below]] $p$, then any filter $G$ containing $p$ will intersect it.
This gives us a $q\in D\cap G$ and thus also some $(\pi,s)\in \tau$.
From $q\leq s$ we find that $s \in G$ 
and from $q\Vdash \sigma=\pi$ we find $\sigma^{G}=\pi^{G}$ and thus $\sigma^{G}\in \tau^{G}$.

To define $p\Vdash \sigma=\tau$ we use this idea along with [[Axiom of Extensionality]].
Say that $p\Vdash \sigma \subseteq \tau$ if and only if 
$$
D_{\pi,s}(\tau) = \{ q \leq p : q \leq s \implies (\exists (\pi',s')\in \tau)\ q\leq s' \land q \Vdash \pi=\pi' \}
$$
is dense below $p$ for all $(\pi,s)\in \sigma$.
Then $p\Vdash \sigma=\tau$
if and only if
$$
p\Vdash \sigma \subseteq \tau\quad %quad
\land\quad %quad
p\Vdash \tau \subseteq \sigma.
$$
This is now enough to give a recursive definition on the rank of [[Name]]s.
This wraps up the atomic formulas.
For composites, we have the following definition:
$$
\begin{align}
p\Vdash \phi \land \psi  & \iff p\Vdash \phi \text{ and } p\Vdash\psi \\
p\Vdash\neg \phi  &  \iff (\forall q\leq p)\, q\not\Vdash\phi \\
p\Vdash (\exists x)\phi(x) & \iff \{ r: (\exists \sigma)\, r\Vdash \phi(\sigma) \} \text{ is dense below } p
\end{align}
$$
By the lemmas about [[Dense Below]], we can show that $\Vdash$ is downwards closed.
Furthermore, one can check that this definition is [[Absolute]] for $M$.
### Properties
Let $G$ be a $\mathbb{P}$-[[Generic Filter]] over $M$.
To find that $\Vdash$ is a [[Forcing Relation]], we need to show that:
$$
\begin{gather}
M[G] \models \varphi(\tau_{1}^{G},\dots,\tau_{k}^{G}) \\
\iff \\
(\exists p\in G)\, M\models (p \Vdash \varphi(\tau_{1},\dots,\tau_{k}))
\end{gather}
$$
We shall first prove this for atomic $\varphi$, 
which boils down to the following two equivalences 
$$
\begin{gather}
\sigma^{G} \subseteq \tau^{G} \iff (\exists p\in G)\ p \Vdash \sigma\subseteq \tau \\
\sigma^{G} \in \tau^{G} \iff (\exists p\in G)\ p\Vdash \sigma \in \tau
\end{gather}
$$
We prove these by induction on terms.
Then we prove it for non-atomic $\varphi$ by induction on formula complexity.
These will together imply that $\Vdash$ is a [[Forcing Relation]].
### Claim 1
$$
\sigma^{G}\subseteq \tau^{G} \iff (\exists p\in G)\ p\Vdash \sigma \subseteq \tau
$$
#### Proof
By $\in$-induction.
##### $\impliedby$
Suppose $p\in G$ forces $\sigma \subseteq \tau$.
Fix $\pi^{G}\in \sigma^{G}$.
Then there is some $s \in G$ with $(\pi,s)\in \sigma$.
As $G$ is a [[Filter]], there is some $q\leq p,s$. 
By assumption, $D_{\pi,s}(\tau)$ is [[Dense Below]] $p$, and so also below $q\in G$.
But then one finds some $r\in D_{\pi,s}(\tau)\cap G$ with $r\leq q$.
By definition of $D_{\pi,s}(\tau)$ and from $r\leq s$, 
we find $(\pi',s')\in \tau$ with $r\leq s'\land r\Vdash \pi=\pi'$.
As $r\in G$, by induction hypothesis find $\pi^{G}=\pi'^{G}$.
Also $s'\in G$ so $\pi'^{G}\in \tau^{G}$ and thus $\pi^{G}\in \tau^{G}$ so $\sigma^{G}\subseteq \tau^{G}$.
##### $\implies$
Fix $r\in \mathbb{P}$ and $(\pi,s)\in \sigma$.

Fix $r\in \mathbb{P}$ and $(\pi_{0},s_{0})\in \tau_{0}$.
Define $\phi_{r,\pi_{0},s_{0}}$ to be 
$$
r\leq s_{0} \land (\forall (\pi_{1},s_{1})\in \tau_{1})\, (\forall q)\, q\leq s_{1} \land q\Vdash \pi_{0}=\pi_{1} \implies q \operatorname{\bot}r
$$
Furthermore, define $\phi_{r}$ to be
$$
(\exists(\pi_{0},s_{0})\in \tau_{0})\, \phi_{r,\pi_{0},s_{0}}
$$
We can check that if $D_{\pi_{0},s_{0}}$ is not dense below $p$
then there is some $r\leq p$ such that $\phi_{r,\pi_{0},s_{0}}$.
We conclude that the following set is [[Dense]]: 
$$
D=\{ p: p \Vdash \tau_{0}\subseteq \tau_{1} \text{ or } \phi_{p} \}
$$
Now suppose $\phi_{r}$ is true for some $r\in G$.
Then find $(\pi_{0},s_{0})\in \tau_{0}$ such that $\phi_{r,\pi_{0},s_{0}}$ is true.
As $r\leq s_{0}$ we find that $s_{0}\in G$ so 
$$
\mathrm{val}(\pi_{0},G) \in \mathrm{val}(\tau_{0},G)
$$
Thus by assumption: 
$$
\mathrm{val}(\pi_{0},G) \in \mathrm{val}(\tau_{1},G)
$$
By definition, find $(\pi_{1},s_{1})\in \tau_{1}$ such that $s_{1}\in G$ and $\mathrm{val}(\pi_{0},G)=\mathrm{val}(\pi_{1},G)$
By induction hypothesis, find $q_{0}\in G$ such that 
$$
q_{0}\Vdash \pi_{0}=\pi_{1}
$$
Finally, find $q\leq q_{0},s_{1}$ with $q\in G$.
Then $\phi_{r,\pi_{0},s_{0}}$ says that $q \operatorname{\bot}r$ which is a contradiction. 
Therefore, $\phi_{r}$ is false for all $r\in G$.
Now by density of $D$ we can find $r\in D\cap G$.
As we know that $\phi_{r}$ is false, it has to be that 
$$
r\Vdash \tau_{0}\subseteq \tau_{1}
$$
which completes the proof.
### Claim 2
Assuming [[#Claim 1]]:
$$
\mathrm{val}(\tau_{0},G) \in \mathrm{val}(\tau_{1},G) \iff (\exists p\in G)\, p\Vdash \tau_{0}\in \tau_{1}
$$
#### Proof
By $\in$-induction.
##### $\implies$
Assume $\mathrm{val}(\tau_{0},G)\in \mathrm{val}(\tau_{1},G)$.
By definition, find some $(\pi,s)\in \tau_{1}$ such that $s \in G$ and $\mathrm{val}(\pi,G)=\mathrm{val}(\tau_{0},G)$.
By [[#Claim 1]] find $r\in G$ such that $r\Vdash \pi=\tau_{0}$.
Now find $p\leq s,r$ such that $p\in G$.
Now we need that 
$$
D=\{ q\leq p : (\exists(\pi,s)\in \tau_{1})\, q\leq s\land q\Vdash \pi=\tau_{0} \}
$$
is [[Dense Below]] $p$.
We can do this by picking $(\pi,s)$ as the witness.
Thus $p\Vdash\tau_{0}\in \tau_{1}$.
#### $\impliedby$
Suppose $p\Vdash\tau_{0}\in \tau_{1}$. 
Then $D$ is [[Dense Below]] $p$ and $p\in G$.
Thus we can find $q\in G\cap D$.
But then there is $(\pi,s)\in \tau_{1}$ with $q\leq s$ (so $s \in G$) such that $q\Vdash\pi=\tau_{0}$
We conclude that 
$$
\mathrm{val}(\pi,G) \in \mathrm{val}(\tau_{1},G)
$$
By [[#Claim 1]], from $q\Vdash\pi=\tau_{0}$ we conclude
$$
\mathrm{val}(\pi,G) = \mathrm{val}(\tau_{0},G)
$$
so we are done.
### Claim 3
If $\Vdash$ satisfies the [[Forcing Relation]] property for $\phi$ and $\psi$ 
then so it does for $\phi \land \psi$.
### Claim 4
If $\Vdash$ satisfies the [[Forcing Relation]] property for $\phi$
then so it does for $\neg \phi$.
#### Proof
Assume 
$$
M[G]\models \phi \iff (\exists p\in G)\, p \Vdash \phi
$$
We want to show: 
$$
M[G] \models \neg \phi \iff (\exists p\in G)\, p\Vdash \neg \phi
$$
##### $\implies$
Consider 
$$
D=\{ p: p\Vdash \phi \text{ or } p \Vdash \neg \phi \}
$$
By definition of $p\Vdash\neg \phi$, this set is [[Dense]].
Thus find some $p\in D\cap G$.
By assumption it follows that 
$$
M[G] \not\models \phi
$$
so by the induction hypothesis $p\not\Vdash\phi$.
But then by definition $p\Vdash\neg \phi$.
##### $\impliedby$
Suppose $p\in G$ and $p\Vdash\neg \phi$.
Assume that $M[G]\models \phi$ (towards a contradiction)
By induction hypothesis, find $r\in G$ such that $r\Vdash\phi$.
Then find some $q\in G$ with $q\leq p,r$.
Now by definition of $p\Vdash\neg \phi$, we have $q\not\Vdash\phi$.
But also $q\leq r\Vdash\phi$ so $q\Vdash\phi$ (by downwards closure of $\Vdash$).
This is a contradiction.
### Claim 5
If $\Vdash$ satisfies the [[Forcing Relation]] property for $\phi$
then so it does for $(\exists x)\,\phi(x)$.
