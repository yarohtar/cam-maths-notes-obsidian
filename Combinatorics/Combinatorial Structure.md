---
aliases:
  - Structure
---
Let $R$ be a [[Algebra/Ring Theory/Ring|Ring]] containing $\mathbb{Q}$.
Let $\mathcal{B}$ be the [[Category]] of finite sets and bijections between them.
Let $\mathcal{B}_{R}$ be the [[Category]] whose objects are pairs $(A,w_{A})$
where $A$ is a finite set and $w_{A}$ is a function $w_{A}:A\to R$
and [[Morphism]]s in $\mathcal{B}_{R}$ are bijections $b:(A,w_{A})\to(B,w_{B})$
such that $w_{A}=w_{B}\circ b$.

A combinatorial structure is a [[Functor]] $F:\mathcal{B}\to \mathcal{B}_{R}$
The map $w_{A}$ is called the weight function.
We may write just $w$ when the context is clear.

Often $w_{A}(a)=1$ for all $a\in A$. 
When weight is not specified, we assume that this is the case.

[[Unlabelled Structure]]
[[Ordinary Generating Function]]
[[Exponential Generating Function]]
[[Combinatorial Union]]
[[Combinatorial Product]]
[[Partition]]
[[Combinatorial Composition]]

### Definition
Given structures $\mathcal{A}=(A,v_{A})$ and $\mathcal{B}(B,v_{B})$ define the following

| Operation         | Symbol                          | Objects                              | Valuation                                      | Conditions                               | [[Ordinary Generating Function\|OGF]]                |
| ----------------- | ------------------------------- | ------------------------------------ | ---------------------------------------------- | ---------------------------------------- | ---------------------------------------------------- |
| Disjoint union    | $\mathcal{A}+\mathcal{B}$       | $A\cup B$                            | $v_{A}\cup v_{B}$                              | $A,B$ disjoint                           | $f_{\mathcal{A}}+f_{\mathcal{B}}$                    |
| Cartesian product | $\mathcal{A}\times \mathcal{B}$ | $A\times B$                          | $v_{A}\cdot v_{B}$                             | none                                     | $f_{\mathcal{A}}\cdot f_{\mathcal{B}}$               |
| Sequence          | $\mathcal{A}^{*}$               | $\bigcup_{k\geq 0} A^{k}$            | $\prod_{i=1}^{k}v_{A}(\alpha_{i})$             | $\varepsilon,A,A\times A \dots$ disjoint | $\frac{1}{1-f_{\mathcal{A}}}$                        |
| Composition       | $\mathcal{B}(\mathcal{A})$      | $\bigcup_{k\geq 0}B_{k}\times A^{k}$ | $w_{B}(\beta)\prod_{i=1}^{k}v_{A}(\alpha_{i})$ | $A,A\times A, \dots$ disjoint            | $b_{0}+\sum_{k\geq 1} b_{k}(f_{\mathcal{A}}(x))^{k}$ |
[[Labelled Product]]
