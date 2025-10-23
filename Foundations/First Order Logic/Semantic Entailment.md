Let $L$ be a [[First-Order Predicate Logic]] language.
Let $S$ be a set of [[Sentence]]s in $L$ and let $t$ be a [[Sentence]] in $L$ 
We say $S$ semantically entails $t$ or $S\models t$ 
if $t$ is [[Satisfied]] in every [[Model]] of $S$.

Furthermore, let $S$ be a set of formulae in $L$ and $t\in L$
Introduce new constants in $L$ 
one for each free variable occurring in $S\cup \{ t \}$
For any $u\in S\cup \{ t \}$, 
let $u'$ be the [[Sentence]] in the new language $L'$ 
obtained from $u$ by replacing free vars with the new constants
Set $S'=\{ s': s \in S \}$ 
We say $S$ entails $t$ or $S\models t$, if $S'\models t'$
