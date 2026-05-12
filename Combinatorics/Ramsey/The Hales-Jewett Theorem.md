Let $m,k\in \mathbb{N}$. 
Then there is some $n\in \mathbb{N}$ such that whenever $[m]^{n}$ is $k$-coloured,
there exists a monochromatic [[Combinatorial Line]].
Write $HJ(m,k)$ for the smallest such $n$.
### Proof
By induction on $m$.
Given $m>1$, assume $HJ(m-1,k)$ exists for all $k$.
Suppose there is no monochromatic line in $[m]^{n}$ for any $n$
We prove for all $r\leq k$ there is some $n$ 
such that $[m]^{n}$ contains $r$ [[Colour-Focused]] lines.
For $r=1$ set $n=HJ(m-1,k)$.
Given $n$ suitable for $r$, let $n'=HJ(m-1,k^{m^{n}})$.
Identify $[m]^{n+n'}$ with $[m]^{n}\times[m]^{n'}$.
There are $k^{m^{n}}$ ways to colour a copy of $[m]^{n}$.
By choice of $n'$, there is a monochromatic line in $[m]^{n'}$.




