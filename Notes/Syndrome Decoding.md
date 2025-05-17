Let $C$ be a $(n,r)$ [[Linear Code]] with [[Parity Check Matrix]] $H$ 
Suppose we receive $x=c+e$ where $c\in C$ is a codeword and $e\in \mathbb{F}_{2}^{n}$ is an 'error pattern'
We form the [[Syndrome]] $Hx$

Suppose we know $C$ is $e$ [[Error correcting]]
Then we tabulate the syndrome $Hz$ for all $z\in \mathbb{F}_{2}^{n}$ with $w(z)\leq e$
If we receive $x$ we search for $Hx$ in our list
If successful, we get $Hx=He$ for some $e\in \mathbb{F}_{2}^{n}$ with $w(e)\leq k$
We decode $x$ as $c=x-e$
Then $c\in C$ as $Hc=Hx-He=0$ and $d(c,x)=w(e)\leq k$
