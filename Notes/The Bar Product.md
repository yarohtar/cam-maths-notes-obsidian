Let $C_{1}$, $C_{2}$ be [[Linear Code]] of length $n$ with $C_{2}\subseteq C_{1}$ 
The bar product is:
$$
C_{1}|C_{2}=\{ (x|x+y):x\in C_{1}, y\in C_{2} \}
$$
            it is a linear code of length $2n$
### Lemma
1. $rank(C_{1}|C_{2})=rank(C_{1})+rank(C_{2})$
2. $w(C_{1}|C_{2})=min\{ 2w(C_{1}),w(C_{2}) \}$
#### Proof
1. Let $x_{1}\dots x_{k}$ be a basis for $C_{1}$. Let $y_{1}\dots y_{l}$ be a basis for $C_{2}$.
   Then $\{ (x_{i}|x_{i}) \}\cup \{ (0|y_{i}) \}$ is a basis for $C_{1}|C_{2}$
   Hence $rank(C_{1}|C_{2})=rank(C_{1})+rank(C_{2})$
2. Let $x\in C_{1}$ and $y\in C_{2}$, not both zero 