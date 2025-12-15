Let $F$ be a [[Field]].
Let $S_{1},S_{2},\dots,S_{n}\subseteq F$ be nonempty and define 
$$
g_{i}(x) = \prod_{s \in S_{i}}(x-s)
$$
Let $f\in F[x_{1},x_{2},\dots,x_{n}]$ be a polynomial satisfying 
$$
f(s) = 0
$$
for all $s \in S_{1}\times S_{2}\times\dots \times S_{n}$.
Then there are some $h_{1},h_{2},\dots h_{n}\in F[x_{1},\dots,x_{n}]$ satisfying 
$$
f(x_{1},\dots,x_{n})=\sum_{i=1}^{n} h_{i}(x_{1},\dots,x_{n}) g_{i}(x_{i})
$$
with total degrees 
$$
\deg h_{i} \leq \deg f - \deg g_{i}
$$
### Proof
