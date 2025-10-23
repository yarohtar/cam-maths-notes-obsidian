Let $\mathcal{L}$ be any [[Language]] and $M$ and $N$ are $\mathcal{L}$-[[Structure]]s.
Then $M$ is a substructure of $N$ if:
- $M\subseteq N$
- $\phi_{M}=\phi_{N}\cap M^{n}$ for any $n$-ary relation symbol $\phi$ 
- $\omega_{M}=\omega_{N}|_{M^{n}}$ for any $n$-ary operation symbol $\omega$

Language of set theory has symbols $\{ \in \}$
### Example
Take
$$
\varepsilon_{0}(x) := (\forall z)(\neg z \in x)
$$
meaning $x=\emptyset$
Also take
$$
\varepsilon_{1}(x):=(\forall z)(z\in x \implies \varepsilon_{0}(z))
$$
meaning $x=\{ \emptyset \}$

Take a model
$$
M\models ZFC
$$
Let $m$ be such that $M\models\varepsilon_{0}(m)$ 
and $n$ such that $M\models\varepsilon_{1}(n)$
Then take $N=M\setminus\{ m \}$
But then $N\models\varepsilon_{0}(n)$ !! 