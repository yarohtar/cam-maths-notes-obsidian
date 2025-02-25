The minimum distance of a [[Binary Code]] $C$ is the smallest [[Hamming distance]] between distinct codewords.

An $[n,m]$ code with minimum distance $d$ is sometimes called $[n,m,d]$

### Lemma
Let $C$ be a code with minimum distance $d$ 
1. Then $C$ is $(d-1)$-[[Error detecting]], but cannot detect $d$ errors
2. $C$ is $\left\lfloor  \frac{d-1}{2}  \right\rfloor$-[[Error correcting]], but cannot correct all sets of $\left\lfloor  \frac{d-1}{2}  \right\rfloor+1$ errors
#### Proof
If $x\in \mathbb{F}_{2}^{n}$ and $c\in C$ with $1\leq d(x,c)\leq d-1$ then $x\not\in C$ so errors detected 
Suppose $c_{1},c_{2}\in C$ with $d(c_{1},c_{2})=d$. Then $c_{1}$ can be corrupted to $c_{2}$ with just $d$ errors, so this set of errors will not be detected.

Let $e=\left\lfloor  \frac{d-1}{2}  \right\rfloor$, so $e\leq \frac{d-1}{2}\leq e+1$