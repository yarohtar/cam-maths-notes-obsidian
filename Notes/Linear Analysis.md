[[Normed Spaces]]
[[Space of Linear Operators]]
[[Dual Spaces]]
[[The Baire Category Theorem]]
[[Spaces of CTS functions]]
[[Hilbert Spaces (PQM)]]
[[Spectral Theory]]

### Books
1. Linear Analysis by Bollobás
2. Topology of Normed Spaces by Jameson
3. Real & Complex Analysis by Rudin


# Definition
For $X$,$Y$ normed, say linear $T:X\to Y$ is compact if $\overline{T(B_{X})}$ is compact.
### Notes
- If $T:X\to Y$ compact, then certainly, $T(B_{X})$ is bounded, so $T$ is continuous.
- For $Y$ complete, $T:X\to Y$ is compact iff $T(B_{X})$ totally bounded
- $T:X\to Y$ compact iff For any $(x_{n})$ in $B_{X}$, there is a subsequence $(x_{n_{i}})$ with $(Tx_{n_{i}})$ converges in $Y$.

### Proposition
$X$, $Y$ normed. With $Y$ complete. Then the compact operators form a closed subspace of $L(X,Y)$.
#### Proof
Subspace: Must show that $S$, $T$, copmact implies $S+T$ compact
Given $(x_{n})$ in $B_{X}$, have subsequence $(x_{n_{i}})$ with $(S{x_{n_{i}}})$ convergent to $y$.
And then $(x_{n_{i}})$ has a subsequence $(x_{m_{i}})$ with $Tx_{m_{i}}\to y'$ say.
So $(S+T)x_{m_{i}}\to y+y'$.
Closed: Let $T_{1},T_{2},\dots$ compact with $T_{n}\to T$. Need $T$ compact.
Given $\epsilon>0$:
Choose $n$ with $\lVert T_{n}-T \rVert<\epsilon$.
Since $T_{n}(B_{X})$ is totally bounded, have
$T_{n}(B_{X})\subseteq \cup_{i=1}^nB(T_{n}(x_{i}),\epsilon)$ for some $x_{1},\dots x_{n}\in B_{X}$
whence $T(B_{X})\subseteq \cup B(T_{m}(x_{i}),2\epsilon)$,
So $T(B_{X})\subseteq \cup B(T(x_{i}),3\epsilon)$
Thus $T(B_{X})$ is totally bounded.

### Note
So any limit of finite rank operators is compact 


### Proposition
$X$, $Y$, $Z$ normed, $S\in L(X,Y)$ and $T\in L(Y,Z)$.
Then:
1. If $S$ is compact $\implies$ $T\circ S$ is compact
2. If $T$ is compact $\implies$ $T\circ S$ is compact
#### Proof
1. Given $(x_{n})$ in $B_{X}$: There is a subsequencce with $(Sx_{n_{i}})$ convergent so $(TSx_{n_{i}})$ convergent ($T$ is continuous)
2. Given $(x_{n})$ in $B_{X}$: have $(Sx_{n})$ bounded, so there is a subsequence with $(TSx_{n_{i}})$ convergent because $T$ is compact.
### Theorem
[[Open Mapping Lemma]]