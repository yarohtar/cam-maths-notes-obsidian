$$
A(n,d)=max\{ m:\exists[n,m,d]\text{-code} \}
$$
ie the size of largest code with parameters $n$ and $d$ 

### Proposition
$$
\frac{2^{n}}{V(n,d-1)}\leq A(n,d)\leq \frac{2^{n}}{V\left( n,\left\lfloor  \frac{d-1}{2}  \right\rfloor  \right)}
$$
#### Proof
[[Hamming's Bound]]
[[Gilbert-Shannon-Varshamov Bound]]

### Example
$$
\frac{2^{10}}{56}\leq A(10,3)\leq \frac{2^{10}}{11}
$$
$$
19\leq A(10,3)\leq 93
$$
$A(10,3)=72$ discovered in 1999. 