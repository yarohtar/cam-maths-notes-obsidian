Let $d\geq 2$ 
$n=2^{d}-1$
Let $H$ be a $d\times n$ matrix whose columns are *all* the nonzero elements of $\mathbb{F}_{2}^{n}$ 
The Hamming $(n,n-d)$ [[Linear Code]] is the linear code with [[Parity Check Matrix]] $H$ (original is $d=3$)

### Lemma 
Let $C$ be a [[Linear Code]] with [[Parity Check Matrix]] $H$. 
Then $w(C)=d$ if and only if
1. any $(d-1)$ columns are linearly independent
2. some $d$ columns are linearly dependent 
#### Proof
Suppose $C$ has length $n$
Then $C=\{ x:Hx=0 \}$
If $H$ has columns $v_{1},\dots ,v_{m}$ 
Then $(x_{1},\dots ,x_{m})\in C$ if and only if $\sum x_{i} v_{i}=0$
### Lemma
The Hamming $(n,n-d)$ [[Linear Code]] $C$ has minimum distance $d(C)=3$ and is a [[Perfect Code]] $1$ [[Error correcting]] code. 
#### Proof
Any $2$ columns of $H$ are linearly independent, but there are some $3$ columns that are linearly dependent so $d(C)=3$
To be perfect, require $\lvert C \rvert=\frac{2^{n}}{V(n,e)}$
Here $n=2^{d}-1$, $e=1$ so it works out 