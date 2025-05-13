Define, using [[The Software Principle]], the sets:
$$
K=\{ w: f_{w,1}(w)\downarrow \}
$$
$$
K_{0}=\{ (w,v):f_{w,1}(v)\downarrow \}
$$
### Theorem
The sets $K$ and $K_{0}$ are [[Computably Enumerable]].
#### Proof
Just run them. If they halt, great. If not then output is $\uparrow$ which is fine.
### Theorem
The sets $K$ and $K_{0}$ are not [[Computable]].
#### Proof
Suppose $K$ was computable. 
Let $\chi$ be the total computable indicator function for $K$.
Define the partial function:
$$
f(w) = \begin{cases}
\uparrow  & w\in K \\
0  & w\not\in K
\end{cases}
$$
