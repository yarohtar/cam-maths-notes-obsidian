Alice chooses a large prime $p$ and a random integer $1<u<p$
Let $g$ be a primitive root $\pmod{p}$.
The public key is $p,g,y=g^{u}\pmod{p}$
The private key is $u$
Let $h:\mathcal{M}\to \{ 1,\dots,p-1 \}$ be a hash function
To send a message $m$ with $0\leq m\leq p-1$, 
Alice randomly chooses $k$ with $1\leq k\leq p-2$ coprime to $p-1$
She computes $r,s$ with $1\leq r\leq p-1$ and $1\leq s\leq p-2$ 
stisfying:
$$
r=g^{k}\pmod{p}
$$