MORAL: Complete spaces are very nice

### Theorem
Let $X$ be a (nonempty) complete metric space, and $O_{1},O_{2}\dots$ a sequence of dense open sets. Then: 
$$
\bigcap_{n=1}^{\infty}O_{n}\neq \emptyset
$$
#### Notation
For open balls write $B(x,\epsilon)=\{ y:d(x,y)<\epsilon \}$
For closed balls write $\overline B(x,\epsilon)=\{ y:d(x,y)\leq \epsilon \}$

#### Proof
$O_{1}\neq \emptyset$ so there is some $\overline B(x_{1},\epsilon_{1})\subseteq O_{1}$ some $x_{1}$ and some $\epsilon_{1}<1$
$O_{2}$ is dense so it meets $B(x_{1},\epsilon_{1})$
 so there is some $\overline B(x_{2},\epsilon_{2})\subseteq O_{2}$ for some $x_{2}$ and some $\epsilon_{2}< \frac{1}{2}$
 Continue inductively and obtain sequence $\overline B(x_{1},\epsilon_{1})\supseteq\dots$
 with $\epsilon _n\to 0$ and 
 $\overline B(x_{n},\epsilon_{n})\subseteq O_{n}$ for all $n$
Now $(x_{n})$ is Cauchy and for any $n,m>N$ have $d(x_{n},x_{m})<2\epsilon_{N}$
Let $x_{n}\to x$
Then $x \in O_{n}$ for all $n$.

### Theorem (alt)
$X$ complete metric, $F_{1},F_{2}\dots$ closed subsets of $X$ with $\bigcup F_{n}=X$. Then some $F_{n}$ has $inF_{n}\neq \emptyset$

### Theorem (altalt)
$X$ complete metric space with $A_{1},A_{2},\dots$ non-dense subsets of $X$. Then $\bigcup A_{n}\neq X$.

[[Meagre]]

### Theorem (altalt)
If $X$ is complete, then $X$ is not a union of [[Meagre]] subsets of $X$.

### Proposition
Let $f_{1},f_{2},\dots \in C[0,1]$ be pointwise bounded.
Then they are uniformly bounded on some interval $(a,b)$.
#### Proof
For $n=1,2,\dots$ let $E_{n}=\{ x\in [0,1] : \forall i \lvert f_{i}(x) \rvert\leq n \}$
Then $E_{n}$ is closed for all $n$. 
Also $\bigcup E_{n}=[0,1]$ (as the $f_{i}$ are pointwise bounded)
Hence some $E_{n}$ has an inte