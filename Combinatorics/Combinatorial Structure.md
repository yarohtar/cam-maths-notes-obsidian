---
aliases:
  - Structure
---
Let $R$ be a [[Algebra/Ring Theory/Ring|Ring]] containing $\mathbb{Q}$.
Let $\mathcal{B}$ be the [[Category]] of finite sets and bijections between them.
Let $\mathcal{B}_{R}$ be the [[Category]] whose objects are pairs $(A,f_{A})$
where $A$ is a finite set and $f_{A}$ is a function $f_{A}:A\to R$
and morphisms in $\mathcal{B}_{R}$ are bijections $b:(A,f_{A})\to(B,f_{B})$
such that $f_{A}=f_{B}\circ b$.
A structure $\mathcal{A}=(A,v)$ consists of a countable set $A$ of combinatorial objects
equipped with a valuation $v:A\to R[x]$ such that 
$$
v(\alpha) = w(\alpha)x^{n}
$$
where $n$ is called the size of $\alpha$ and $w(\alpha)\in R$ is called the weight 
(often $w(\alpha)=1$ for all $\alpha$)
and moreover 
$$
A_{n} = \{ \alpha \in A \text{ of size }n \}
$$
is finite for all $n$.
We define its [[Ordinary Generating Function]]
and [[Exponential Generating Function]]
### Definition
Given structures $\mathcal{A}=(A,v_{A})$ and $\mathcal{B}(B,v_{B})$ define the following

| Operation         | Symbol                          | Objects                              | Valuation                                      | Conditions                               | [[Ordinary Generating Function\|OGF]]                |
| ----------------- | ------------------------------- | ------------------------------------ | ---------------------------------------------- | ---------------------------------------- | ---------------------------------------------------- |
| Disjoint union    | $\mathcal{A}+\mathcal{B}$       | $A\cup B$                            | $v_{A}\cup v_{B}$                              | $A,B$ disjoint                           | $f_{\mathcal{A}}+f_{\mathcal{B}}$                    |
| Cartesian product | $\mathcal{A}\times \mathcal{B}$ | $A\times B$                          | $v_{A}\cdot v_{B}$                             | none                                     | $f_{\mathcal{A}}\cdot f_{\mathcal{B}}$               |
| Sequence          | $\mathcal{A}^{*}$               | $\bigcup_{k\geq 0} A^{k}$            | $\prod_{i=1}^{k}v_{A}(\alpha_{i})$             | $\varepsilon,A,A\times A \dots$ disjoint | $\frac{1}{1-f_{\mathcal{A}}}$                        |
| Composition       | $\mathcal{B}(\mathcal{A})$      | $\bigcup_{k\geq 0}B_{k}\times A^{k}$ | $w_{B}(\beta)\prod_{i=1}^{k}v_{A}(\alpha_{i})$ | $A,A\times A, \dots$ disjoint            | $b_{0}+\sum_{k\geq 1} b_{k}(f_{\mathcal{A}}(x))^{k}$ |
[[Labelled Product]]
