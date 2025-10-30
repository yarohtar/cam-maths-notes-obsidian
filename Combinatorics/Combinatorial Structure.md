---
aliases:
  - Structure
---
Let $R$ be a [[Algebra/Ring Theory/Ring|Ring]] containing $\mathbb{Q}$.
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
is finite for all $n$, so the [[Generating Function]]
$$
f_{\mathcal{A}}(x) = \sum_{\alpha \in A} v(\alpha) \in R[[x]]
$$
is well defined, as is the exponential generating function:
$$
\tilde{f}_{\mathcal{A}} (x) = \sum_{n\geq 0} \sum_{\alpha \in A_{n}} \frac{ v(\alpha) }{ n! }
$$
### Definition
Given structures $\mathcal{A}=(A,v_{A})$ and $\mathcal{B}(B,v_{B})$ define the following

| Operation         | Symbol                          | Object                               | Valuation                                      | Conditions                               | OGF                                                  |
| ----------------- | ------------------------------- | ------------------------------------ | ---------------------------------------------- | ---------------------------------------- | ---------------------------------------------------- |
| Disjoint union    | $\mathcal{A}+\mathcal{B}$       | $A\cup B$                            | $v_{A}\cup v_{B}$                              | $A,B$ disjoint                           | $f_{\mathcal{A}}+f_{\mathcal{B}}$                    |
| Cartesian product | $\mathcal{A}\times \mathcal{B}$ | $A\times B$                          | $v_{A}\cdot v_{B}$                             | none                                     | $f_{\mathcal{A}}\cdot f_{\mathcal{B}}$               |
| Sequence          | $\mathcal{A}^{*}$               | $\bigcup_{k\geq 0} A^{k}$            | $\prod_{i=1}^{k}v_{A}(\alpha_{i})$             | $\varepsilon,A,A\times A \dots$ disjoint | $\frac{1}{1-f_{\mathcal{A}}}$                        |
| Composition       | $\mathcal{B}(\mathcal{A})$      | $\bigcup_{k\geq 0}B_{k}\times A^{k}$ | $w_{B}(B_{k})\prod_{i=1}^{k}v_{A}(\alpha_{i})$ | $A,A\times A, \dots$ disjoint            | $b_{0}+\sum_{k\geq 1} b_{k}(f_{\mathcal{A}}(x))^{k}$ |
[[Labeled Product]]