### Notation
1. $0\in\mathbb{N}$ with $n=\{ 0,\dots,n-1 \}$, $0=\emptyset$
2. $X$ finite set of symbols
   We call $X^n$ the set of $X$-strings of length $n$.
   Set theoretic convention:
   $\alpha\in X^n\implies \alpha:n\to X$; write $|\alpha|=n$
3. Empty string $\varepsilon : \emptyset\to X$
4. $X^*=\cup_{n\in \mathbb{N}}X^n$ the set of $X$-strings
5. If $|\alpha|=n$ and $k\leq n$, then $\alpha|_{k}$ is the unique initial segment of $\alpha$ with length $k$.
6. $X^+=X^*\\ \{ \varepsilon \}$ The set of nonempty strings
7. $\alpha \beta$ the concatenation of $\alpha$ and $\beta$ 
8. Write $\alpha x$ for $\alpha \beta$ when $\beta$ is string containing only $x$ 
9. $x^n$ string of length $n$ containing only $x$ 
10. If $f:X\to Y$ then there is a natural $\hat{f}:X^*\to Y^*$
11. Set is infinite if $\mathbb{N}$ injects into it
12. Set is countable if its empty or $\mathbb{N}$ surjects onto it

[[Rewrite Systems]]
[[Grammars]]

### Definition
Regular concatenation grammar RCG from $G=(\Sigma,V,S,P)$ and $G'=(\Sigma,V',S',P')$
Define $P^+=P'\cup P-\{ A\to a; A\to a\in P \}\cup \{ A\to aS';A\to a\in P \}$
and get the new grammar $G^+ =(\Sigma,V\cup V',S,P^+)$
### Definition
Regular union grammar RUG
$P^+=P\cup P' \cup \{ T\to \alpha;S\to \alpha \in P \} \cup \{ T\to \alpha;S'\to \alpha \in P' \}$

### Proposition
If $G,G'$ are regular and $V\cap V'=\emptyset$, then 
1. If $H$ RCG, then $\mathcal{L}(H)=\mathcal{L}(G)\mathcal{L}(G')$
2. If $H$ RUG, then $\mathcal{L}(H)=\mathcal{L}(G)\cup \mathcal{L}(G')$

[[Deterministic Automata]]