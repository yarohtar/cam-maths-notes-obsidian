Sequence defined by 
$$
F_{n+2}=F_{n+1}+F_{n}
$$
and initial condition $F_{1}=F_{2}=1$

## Theorem
The number of ways of tiling $1\times n$ rectangle 
with $1\times 1$ and $1\times 2$ tiles is $F_{n+1}$.
This has generating function
$$
\sum_{n=0}F_{n+1}x^{n} = \frac{1}{1-x-x^{2}} \in \mathbb{C}[[x]]
$$
and 
$$
F_{n} = \frac{1}{\sqrt{ 5 }} \left( \left( \frac{ 1+\sqrt{ 5 } }{ 2 } \right)^{n} + \left( \frac{ 1-\sqrt{ 5 } }{ 2 } \right)^{n} \right)
$$
### Proof
First bit by same recurrence relation
Note that $(x+x^{2})^{i}$ is the generating function for tiling with precisely $i$ tiles
So:
$$
\sum_{n\geq 0} F_{n+1} x^{n} = 1 + (x+x^{2}) + (x+x^{2})^{2} + \dots
$$
Thus the generating function is:
$$
\sum_{n\geq 0} F_{n+1}x^{n+1} = \frac{ x }{ 1-x-x^{2} }
$$
## Theorem
$$
F_{n+1} = \sum_{i=0}^{\lfloor n/2 \rfloor } \binom{ n-i }{ i }
$$
### Proof
Count tillings with $i$ $1\times 2$ tiles.
## Theorem
Given prime $p>2$
$$
p|F_{p+1} + F_{p-1} -1 
$$
### Proof
It turns out that $F_{n+1}+F_{n-1}$ is the number of ways of tilling a $1\times n$ cycle 
So the number of cyclically distinct tilings of a $1\times p$ cycle,
when $p$ is prime, is:
$$
1+ \left( \frac{ F_{p+1} + F_{p-1} - 1 }{ p } \right) \in \mathbb{N}
$$
Phrase this as a [[Burnside's Lemma (Orbit-Counting Lemma)]]

Thus $p$ has to divide $F_{p+1}+F_{p-1}-1$

$\sqrt{ 5 }$ exists $\pmod{p}$ 
if and only if
$$
\left( \frac{ 5 }{ p } \right) = \frac{ p }{ 5 } = 1
$$
if and only if
$$
p \equiv \pm 1 \pmod{5}
$$
## Theorem (Wall, 1960)
If $p$ is prime and $p\equiv \pm 1\pmod{5}$, then $F_{p-1}\equiv 0\pmod{p}$ and $F_{p+1}\equiv 1\pmod{p}$
and $F_{n}\pmod{p}$ has period $k(p)|p-1$
### Proof
Apply previous theorems, and use [[Fermat's Little Theorem]]