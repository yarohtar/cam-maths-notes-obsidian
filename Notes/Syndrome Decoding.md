Let $C$ be a $(n,r)$ [[Linear Code]] with [[Parity Check Matrix]] $H$ 
Then $C=\{ c\in \mathbb{F}_{2}^{n}: Hc=0 \}$ where $c$ is a column vector.

Suppose we receive $x=c+e$ where $c\in C$ is a codeword and $e\in \mathbb{F}_{2}^{n}$ is an 'error pattern'

We complete the syndrome $Hx$
Suppose we know $C$ is $k$ [[Error correcting]]
Then we tabulate the syndrome $He$ for all $e\in \mathbb{F}_{2}^{n}$ with $w(e)\leq k$
If we receive $x$ we search for $Hx$ in our list
