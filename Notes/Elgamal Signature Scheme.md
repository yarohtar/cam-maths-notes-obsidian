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
$$
h(m)=ur+ks\pmod{p-1}
$$
Since $k$ is coprime to $p-1$, we can always find $s$.
Alice signs the message with $(r,s)$
Now:
$$
g^{h(m)}=g^{ur+ks}=(g^{u})^{r}(g^{k})^{s}=y^{r}r^{s}\pmod{p}
$$
so Bob accepts a signature if $g^{h(m)}=y^{r}r^{s}\pmod{p}$
Any obvious attempt at forging involves the discrete log

### Lemma
Let $a,b,m\in \mathbb{N}$ and consider $ax=b\pmod{m}$. 
This has either no solutions or $\operatorname{gcd}(a,m)$ solutions for $x$
### Corollary
Alice HAS TO choose different $k$ each time.
Suppose she sends $m_{1}$ and $m_{2}$ using the same $k$
with signatures $(r,s_{1})$ and $(r,s_{2})$
Then:
