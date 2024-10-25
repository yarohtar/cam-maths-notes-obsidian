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