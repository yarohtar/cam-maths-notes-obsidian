## Language
The language is specified by a disjoint pair of sets:
$\Omega$ the set of operation symbols
$\Pi$ the set of predicate symbols
and an arity function $\alpha:\Omega \cup \Pi \to \mathbb{N}_{0}=\{ 0 \}\cup \mathbb{N}$

The language $L=L(\Omega,\Pi)$ consists of the following:
### Variables
This is a countably infinite set disjoint from $\Omega$ and $\Pi$
We denote variables by $x_{1},x_{2},\dots$ or $x,y,z\dots$

### Terms
Or $\Omega$-terms are defined inductively:
1. Every variable is a term
2. if $\omega \in \Omega$ with $n=\alpha(\omega)$ and $t_{1},t_{2},\dots,t_{n}$ are terms then $\omega t_{1}t_{2},\dots t_{n}$ is a term
### Atomic formulae
Two kinds:
1. If $s$, $t$ are terms then $(s=t)$ is an atomic formulae
2. if $\phi \in\Pi$ with $n=\alpha(\phi)$ and $t_{1},t_{2},\dots,t_{n}$ are terms then $\phi t_{1}t_{2}\dots t_{n}$ is an atomic formulae.
### Formulae
1. Atomic formulae
2. $\bot$ is a formulae
3. If $p$, $q$ are formulae then so is $(p \implies q)$
4. If $p$ is a formula and $x$ is a free variable in $p$ then $(\forall x)p$ is a formula
### Definition (free variable)
Any occurrence of a variable in a formula can be either free or bound. 
1. Any occurrence of any variable in an atomic formula is free
2. Given formulae $p$, $q$ any occurrence of a variable in $p$ or $q$ remains an occurrence of the same type in $(p\implies q)$
3. If $p$ is a formulae and $x$ has at least one free occurrence in $p$ then every free occurence of $x$ in $p$ becomes bound in $(\forall x)p$ (everything else is unchanged)
We let $FV(p)$ be the set of free variables in a formula $p$ i.e. variables that have at least one free occurrence in $p$ 
### Definition
A formula with no free variables is called a sentence.
### Definition
A structure in a first-order language $L=L(\Omega,\Pi)$ (or $L$-structure) is a non-empty set $A$ together with functions $\omega_{A}:A^{n}\to A$
(where $\omega \in \Omega$ and $n=\alpha(\omega)$)
and subset $\phi_{A}\subseteq A^{n}$ (where $\phi \in\Pi$ and $n=\alpha(\phi)$)
(or identifying a subset with its indicator function $\phi_{A}:A^{n}\to \{ 0,1 \}$)
#### Note 
If $\alpha(\omega)=0$ then $\omega$ is called a constant. Its interpretation in a structure is $\omega_{A}:A^{0}\to A$ i.e. an element $\omega_{A}\in A$