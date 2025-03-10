A code $C\subseteq \mathbb{F}_{2}^{n}$ is a cyclic code if it is [[Linear Code]] and 
$(a_{0},\dots,a_{n-1})\in C\implies(a_{1},\dots,a_{n-1},a_{0})\in C$
We identify $\mathbb{F}_{2}^{n}$ with the [[Ring]] $\frac{\mathbb{F}_{2}[X]}{(X^{n}-1)}$ via
$$
\pi(a_{0},a_{1},\dots,a_{n-1})\to a_{0}+a_{1}X+\dots+a_{n-1}X^{n-1} 
$$
### Lemma
A code $C$ is cyclic iff $\mathcal{C}=\pi(C)$ satisfies
1. $0\in \mathcal{C}$
2. $f,g\in \mathcal{C}$ then $f+g\in \mathcal{C}$
3. $f\in \mathcal{C}$