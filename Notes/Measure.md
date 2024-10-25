Given a set $E$ and a [[sigma-algebra]] $\mathcal{E}$ on it, the pair $(E,\mathcal{E})$ is called a measurable space, while each $A\in \mathcal{E}$ is called a measurable set. 

A function $\mu:\mathcal{E}\to[0,\infty]$ with $\mu(\emptyset)=0$ is called a measure if for any sequence $(A_{n})$ of disjoint elements of $\mathcal{E}$,
$$
\mu\left( \bigcup_{n}A_{n} \right)=\sum_{n}\mu(A_{n})
$$
This property is called countable additivity. 

The triple $(E,\mathcal{E},\mu)$ is called a measure space.

### Properties
- If $\mu(E)=1$ then $\mu$ is a probability measure and $(E,\mathcal{E},\mu)$ is a [[Probability Space]], often denoted  by $(\Omega,\mathcal{F},\mathbb{P})$
- If $\mu(E)<\infty$, then $\mu$ is a finite measure
- If there exists a sequence of sets $(E_{n})$ in $\mathcal{E}$ with $\mu(E_{n})<\infty$ for all $n$ and $\bigcup_{n}E_{n}=E$ then $\mu$ is a $\sigma$-finite measure

[[Set Function]]
[[Algebra (of sets)]]
[[Ring (of sets)]]
[[Carathéodory's Extension Theorem]]
[[Uniqueness of Measures]]
[[Borel Sets]]
[[Lebesgue Measure]]