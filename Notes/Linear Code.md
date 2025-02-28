A [[Code]] $C\subseteq \mathbb{F}_{2}^{n}$ is linear if
1. $0\in C$
2. if $x,y\in C$ then $x+y\in C$

[[Rank of a Linear Code]]
A code of length $n$ and rank $k$ is called an $(n,k)$ code. 

Say $C$ has a basis $v_{1},\dots,v_{k}$
Then $C=\left\{  \sum \lambda_{i}v_{i}:\lambda_{i}\in \mathbb{F}_{2}  \right\}$ so $\lvert C \rvert=2^{k}$
i.e. an $(n,k)$ code is an $[n,2^{k}]$ code

The information rate is $\frac{k}{n}$

We define $x.y=\sum_{i}^{n}x_{i}y_{i}$
[[Parity Check Code]]
[[Dual Code]]
[[Generator Matrix]]
[[Parity Check Matrix]]
### Lemma
Every $(n,k)$ linear code is equivalent to a linear code with [[Generator Matrix]] of form $(I_{k}|B)$
#### Proof
We can perform row operations:
- swap 2 rows
- add one row to another
By Gaussian elimination we get $G$, the generator matrix in row form:
$$
G=\begin{pmatrix}
1 & * & * & \dots & * \\
0 & 1 & * & \dots & * \\
0 & 0 & 1 & \dots & *  \\
\vdots & \vdots & \vdots & 
\end{pmatrix}
$$