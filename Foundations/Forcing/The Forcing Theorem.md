Let $M$ be a countable [[Transitive Model]] and $\mathbb{P}\in M$ a [[Forcing Partial Order]].
Then there is an [[Absolute]] [[Forcing Relation]] $\Vdash$ on $\mathbb{P}\times \mathrm{Se nt}_{\mathbb{P},M}$.
## Proof (chunky one)
We first define the [[Forcing Relation]] $\Vdash$ on atomic formulas.
Fix some $p\in \mathbb{P}$ and $\tau_{0},\tau_{1}\in \mathrm{Name}^{\mathbb{P}}$.
Let $\{ i,j \}=\{ 0,1 \}$ and denote
$$
D_{\pi_{i},s_{i}} = \{ q\leq p : q\leq s_{i} \implies (\exists (\pi_{j},s_{j})\in \tau_{j})\, q\leq s_{j} \land q \Vdash \pi_{i}=\pi_{j} \}
$$
Then we define $p\Vdash\tau_{0}=\tau_{1}$ to mean 
$$
\begin{gather}
(\forall(\pi_{0},s_{0})\in \tau_{0})\, D_{\pi_{0},s_{0}} \text{ is dense below }p \\
\text{and} \\
(\forall(\pi_{1},s_{1})\in \tau_{1})\, D_{\pi_{1},s_{1}} \text{ is dense below }p
\end{gather}
$$
As a helper, we define $p\Vdash\tau_{0}\subseteq \tau_{1}$ to be 
$$
(\forall(\pi_{0},s_{0})\in \tau_{0})\, D_{\pi_{0},s_{0}}\text{ is dense below }p
$$
Now define $p\Vdash\tau_{0}\in \tau_{1}$ to be 
$$
\{ q\leq p : (\exists(\pi,s)\in \tau_{1})\, q\leq s\land q\Vdash \pi=\tau_{0} \} \text{ is dense below }p
$$
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

Now let $G$ be a $\mathbb{P}$-[[Generic Filter]] over $M$.
We will prove the following claims by a (double) induction.
These will together imply that $\Vdash$ is a [[Forcing Relation]].
### Claim 1
$$
\mathrm{val}(\tau_{0},G) \subseteq \mathrm{val}(\tau_{1},G) \iff (\exists p\in G)\, p \Vdash \tau_{0}\subseteq \tau_{1}
$$
#### Proof

### Claim 2
Assuming [[#Claim 1]]:
$$
\mathrm{val}(\tau_{0},G) \in \mathrm{val}(\tau_{1},G) \iff (\exists p\in G)\, p\Vdash \tau_{0}\in \tau_{1}
$$
#### Proof
We want to show 
$$
\mathrm{val}(\tau_{0},G) \in \mathrm{val}(\tau_{1},G) \iff (\exists p\in G)\, p\Vdash \tau_{0}\in \tau_{1}
$$
##### $\implies$
Assume $\mathrm{val}(\tau_{0},G)\in \mathrm{val}(\tau_{1},G)$.
By definition, find some $(\pi,s)\in \tau_{1}$ such that $s \in G$ and $\mathrm{val}(\pi,G)=\mathrm{val}(\tau_{0},G)$.
By [[#Claim 1]] find $r\in G$ such that $r\Vdash \pi=\tau_{0}$.
Now find $p\leq s,r$ such that $p\in G$.
Now we need that 
$$
\{ q\leq p : (\exists(\pi,s)\in \tau_{1})\, q\leq s\land q\Vdash \pi=\tau_{0} \}
$$
is [[Dense Below]] $p$.
We can do this by 

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
