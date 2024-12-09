Suppose we use some numerical scheme in the spatial coordinates and get
$$
u'=Au
$$
We might be tempted to say $u=e^{tA}u$, and then $u^{n+1}=e^{tA}u^{n}$
Unfortunately, computing and controlling the error of $e^{tA}$ is complicated in general, however for some special cases we might get lucky.

Suppose $A=B+C$
Then
$$
e^{ tA }=e^{ tB }e^{ tC }+\frac{1}{2}t^{2}(CB-BC)+O(t^{3})
$$
If $B$ and $C$ commute, then $e^{tA}=e^{tB}e^{ tC }$
#### Proof
Taylor expand.

### Splitting

This allows for writing:
$$
u^{n+1}=e^{tB}e^{tC}u^{n}
$$
where we can now use
$$
r(z)=\left( 1+\frac{z}{2} \right)\left( 1-\frac{z}{2} \right)^{-1}
$$
to approximate the exponential.

In particular in the case of [[Crank-Nicolson method for diffusion equation]]