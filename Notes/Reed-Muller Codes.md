Let $X=\mathbb{F}_{2}^{n}=\{ p_{1},\dots,p_{n} \}$ where $n=2^{d}$
For each $A\subseteq X$  we get a vector $\mathbb{1}_{A}\in \mathbb{F}_{2}^{n}$ by the rule:
$(\mathbb{1}_{A})_{i}=1$ iff $p_{i}\in A$ (i.e. its an indicator of $A$)

For $A,B\subseteq X$ we have:
$$
\begin{gather}
\mathbb{1}_{A}+\mathbb{1}_{B}=\mathbb{1}_{A}\triangle\mathbb{1}_{B}\\
\mathbb{1}_{A}\land \mathbb{1}_{B}=\mathbb{1}_{A}\cap \mathbb{1}_{B}\\
w(\mathbb{1}_{A})=\lvert A \rvert 
\end{gather}
$$
Let $v_{0}=\mathbb{1}_{A}(1,1,\dots 1)$
For $1\leq i\leq d$ let $v_{i}=\mathbb{1}_{H_{i}}$ where $H_{i}=\{ p \in X: p_{i}=0 \}$

### Definition
Reed-Muller code $RM(d,r)$ of order $r$ and length $n=2^{d}$ is the vector subspace of $\mathbb{F}_{2}^{n}$ spanned by $v_{0}$ and wedge products of at most $r$ of the $v_{i}$.

### Example
$$
\begin{gather}
X = \{ 000,001, 010,011,100,101,110,111 \}\\
v_{0}=( 1,1,1,1,1,1,1,1)\\
v_{1}=( 1,1,1,1,0,0,0,0)\\
v_{2}=( 1,1,0,0,1,1,0,0)\\
v_{3}=( 1,0,1,0,1,0,1,0)\\
v_{1}\land v_{2}=(1,1,0,0,0,0,0,0)\\
v_{2}\land v_{3}=(1,0,0,0,1,0,0,0)\\
v_{1}\land v_{3}=(1,0,1,0,0,0,0,0)\\
v_{1}\land v_{2}\land v_{3}=(1,0,0,0,0,0,0,0)
\end{gather}
$$
$RM(3,0)$ is spanned by $v_{0}$. It is the repetition code of length 8
$RM(3,1)$ is spanned by $v_{0},v_{1},v_{2},v_{3}$. Deleting the first component of each codeword gives [[Hamming's Original Code]]
$RM(3,2)$ is spanned by all the previous plus $v_{1}\land v_{2}$, etc.
$RM(3,3)=\mathbb{F}_{2}^{8}$
 
### Theorem
1. The vector $v_{i_{1}}\wedge\dots \wedge v_{i_{s}}$ for $1\leq i_{1}<\dots<i_{s}\leq d$ and $0\leq s\leq d$ are a basis for $\mathbb{F}_{2}^{n}$
2. $RM(d,r)$ has rank $\sum_{s=0}^{r}{d \choose s}$
3. $RM(d,r)=RM(d-1,r)\mid RM(d-1,r-1)$
4. $RM(d,r)$ has weight $2^{d-r}$
#### Proof
1. We have a set of $\sum_{s=0}^{d}{d \choose s}=(1+1)^{d}=2^{d}$ vectors
   So it suffices to show they span $\mathbb{F}_{2}^{n}$, equivalently $RM(n,d)=\mathbb{F}_{2}^{n}$
   Let $p \in X$
   Let 
   $a$
      